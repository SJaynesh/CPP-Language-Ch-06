# Inheritance 

<br><br>

## What is Inheritance? 

<br>

> * Inheritance allows a **new class (derived or child class ) to inherit properites and behaviour from an existing class(base or parent class)**
> * Passing a data into another class from one class.
> * To Share data from one class to another class.

<br><br>

## Types of Inheritance : 

<br>


> 1) `Simple / Single Inheritance`
> 2) `Multilevel Inheritance`
> 3) `Hierarchical Inheritance`
> 4) `Multiple Inheritance`
> 5) `Hybrid Inheritance`

<br><br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/a50a3004-adcc-47e5-881b-6d00d58389e5.png" width=150% height=100%></p>

<br>

### 1) Parent Class :

> * The class whose properties and methods are inherited. Also known as the **base class** or **super class**.
> * Here main class which data will be shared is called parent class/super class/base class.

<br>

### 2) Child Class :

> * The class that inherits properties and methods from the base class. Also known as the **derived class** or **sub class**.
> * The class which consumes data of another class is called child class/sub class/derived class.

<br><br>

## Syntax: 

<br>

![inheritance](https://github.com/user-attachments/assets/49723fb3-5f6e-42b9-b35f-b6b0dfb00204)


<br><br>

## 1) Simple / Single Inheritance : 

<br>

> * `In single inheritance, a class can inherit from only one class.`

<br>

> `Minimum class : ` 2 <br>
> `Maximum class : ` 2 <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/e8be4f7e-c72c-490b-9221-0f4552de175a.png" width=60% height=50%></p>

<br>


<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/1a7f4fad-be30-4c50-984a-591081aee40c.png" width=60% height=50%></p>

<br>

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

<br><br>

## 2) Multilevel Inheritance : 

<br>

> * `In multilevel inheritance, a class can inherit from a derived class, making the inheritance chain longer.`

<br>

> `Minimum class : ` 3 <br>
> `Maximum class : ` N number <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/b391c75c-308b-4d4d-87f4-6eeed8ef9cf0.png" width=60% height=50%></p>

<br><br>

## 3) Hierarchical Inheritance : 

<br>

> * `Hierarchical inheritance to provide only one Parent class and multiple child class.`
> * Multiple derived classes inherit from a single base class.

<br>

> `Minimum class : ` 3 <br>
> `Maximum class : ` N number <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/2ce29599-e97d-4715-8de7-6ebcfb09df57.png" width=60% height=50%></p>

<br><br>

## 4) Multiple Inheritance : 

<br>

> * `A class can inherit attributes and methods from more than one base class.`

<br>

> `Minimum class : ` 3 <br>
> `Maximum class : ` N number <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/c7ee1a62-7164-4b14-aa13-e034c652107c.png" width=60% height=50%></p>

<br><br>

## 5) Hybrid Inheritance : 

<br>

> * `Two Inheritance combination to create One inheritance it's called Hybrid inheritance.`

> `Minimum class : ` 4 <br>
> `Maximum class : ` N number <br>

<br>

<p><img src = "https://github.com/SJaynesh/CPP-Languge-Ch-06/assets/115562979/71cccca0-4c61-4a6b-85a8-3f471cfecf05.png" width=60% height=50%></p>

<br><br>

## Error of Ambiguity (Duplicate):

<br>

> * When we get the request of same method or attribute from multiple class which are not directly connected.
> * same method from different sources.

<br>

> * ` ambiguity == duplication == repetition `

<br>

## This error occurs only in two inheritances.

<br>

> 1. Multiple
> 2. Hybrid

<br>

## Solution of Ambiguity :

<br>

### 1. Temporory :

<br>

> * - using scope resolution operator (::)

<br>

### 2. Permenant : 

<br>

> * - using virtual method







