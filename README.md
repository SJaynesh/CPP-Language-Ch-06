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

<br>


<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/1a7f4fad-be30-4c50-984a-591081aee40c.png" width=60% height=50%></p>

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

<br>

## 2) Multilevel inheritance : 
> * `In multilevel inheritance, a class can inherit from a derived class, making the inheritance chain longer.`

<br>

> `Minimum class : ` 3 <br>
> `Maximum class : ` Unlimited <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/b391c75c-308b-4d4d-87f4-6eeed8ef9cf0.png" width=60% height=50%></p>

<br>

## 3) Hierarchical inheritance : 
> * `Hierarchical inheritance to provide only one Parent class and multiple child class.`
> * Multiple derived classes inherit from a single base class.

<br>

> `Minimum class : ` 3 <br>
> `Maximum class : ` Unlimited <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/2ce29599-e97d-4715-8de7-6ebcfb09df57.png" width=60% height=50%></p>

<br>

## 4) Multiple inheritance : 
> * `A class can inherit attributes and methods from more than one base class.`

<br>

> `Minimum class : ` 3 <br>
> `Maximum class : ` Unlimited <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/c7ee1a62-7164-4b14-aa13-e034c652107c.png" width=60% height=50%></p>

<br>

## 5) Hybrid inheritance : 

<br>

> `Minimum class : ` 4 <br>
> `Maximum class : ` Unlimited <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/71cccca0-4c61-4a6b-85a8-3f471cfecf05.png" width=60% height=50%></p>

<br>

## Error of Ambiguity (Duplicate):
> * When we get the request of same method or attribute from multiple class which are not directly connected.
> * same method from different sources.

<br>

> * ` ambiguity == duplication == repetition `

<br>

## This error occurs only in two inheritances.
> 1. Multiple
> 2. Hybrid

<br>

## Solution of Ambiguity :

<br>

### 1. Temporory :
> * - using scope resolution operator (::)

<br>

### 2. Permenant : 
> * - using virtual method







