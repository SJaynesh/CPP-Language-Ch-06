# Inheritance :

> * `To Share data from one class to another class.`
> * Here main class which data will be shared is called parent class/super class/base class.
> * The class which consumes data of another class is called child class/sub class/derived class.

<br>

## `It can be done by following below syntax :`

<br>

<pre>
    
    class A {
				
      //dataOfClassA
		
    }
  
   class B : [access modifier-(default private)] A {
		
    //dataOfClassB
		
    }
  
</pre>

<br>

> * Here data of class A is shared with class B thus class B can possess both class's data.
> * Parent class can't access child class's data but child class can access parent's data.

<br>

## Types of Inheritance : 

> 1) Simple / Single inheritance
> 2) Multilevel inheritance
> 3) Hierarchical inheritance
> 4) Multiple inheritance
> 5) Hybrid inheritance

<br>

## 1) Simple / Single inheritance : 
> * `In single inheritance, a class can inherit from only one class.`

<br>

> `Minimum class : ` 2 <br>
> `Maximum class : ` 2 <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/e8be4f7e-c72c-490b-9221-0f4552de175a.png" width=60% height=50%></p>

<pre>
  #include<iostream>
  using namespace std;
  
  class A {
  	
  	private :
  		int a;
  		
  	public :
  		
  		void setDataA() {
  			cout << "Enter A : ";
  			cin >> a;
  		}	
  		
  		void getDataA() {
  			cout << endl << "\tA : " << a << endl;
  		}
  };
  
  class B : public A{
  	
  	private : 
  		int b;
  		
  	public : 
  		 
  		 void setDataB() {
  		 	cout << "Enter B : " ;
  		 	cin >> b;
  		 }
  		 
  		 void getDataB() {
  		 	cout << endl << "\tB : " << b << endl;
  		 }
  };


int main () {
	
	B b1;
	
	b1.setDataA();
	b1.setDataB();
	b1.getDataA();
	b1.getDataB();
	
}
</pre>
    
## 2) Multilevel inheritance : 
> * `In multilevel inheritance, a class can inherit from a derived class, making the inheritance chain longer.`

<br>

> `Minimum class : ` 3 <br>
> `Maximum class : ` Unlimited <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/b391c75c-308b-4d4d-87f4-6eeed8ef9cf0.png" width=60% height=50%></p>




