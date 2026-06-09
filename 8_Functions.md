# Functions:

# QUESTION 1: Calculator Operations (+,-,*,/,%)
#### Create four (04) separate functions, each of which gets two integer values as parameters and returns the subtraction, multiplication, division, and modulus (remainder) of those two values, respectively.
#### then call these functions in the main() function and print the values returned by them.


## CODE:

		#include <iostream> 
		using namespace std; 
		int addition(int a, int b){
		int sum = a + b; 
		return sum;
		}
		int subtraction(int a, int b){ 
		int sub = a - b;
		return sub;
		}
		int multiplication(int a, int b){ 
		int mul = a*b;
		return mul;
		}
		float division(int a, int b){ 
		float div= (float) a/b; 
		return div;
		}
		int mod(int a, int b){
		int rem = a%b; 
		return rem;
		}
		int main(){
		int a, b;
		
		
		cout << "Enter 1st Value: ";
		cin >> a;
		cout << "Enter 2nd Value: ";
		cin >> b;
		
		cout << "\nAddition = " << addition(a,b); 
		cout << "\nSubtraction = " << subtraction(a,b); 
		cout << "\nMultiplication = " << multiplication(a,b); 
		cout << "\nDivision = " << division(a,b); 
		cout << "\nModulus = " << mod(a,b);
		
		return  0;
		}

# OUTPUT:

<img width="619" height="317" alt="image" src="https://github.com/user-attachments/assets/6a5fab66-0b23-40fe-be54-e7178191c32b" />




# QUESTION 2: Power:

#### Write a C++ program that defines a function power to calculate the power of a number. 
#### double power(double base, int exponent) {

## Code:

		#include <iostream> 
		using namespace std;
		double power(double base, int exponent){ 
		int result = 1;
		for(int i=1 ; i<=exponent ; i++){
		result *= base;
		}
		}
		int main(){
		int base, exp; 
		cout << "Enter base:"; 
		cin>>base;
		cout << "Enter exponent: "; 
		cin >> exp;
		if(exp>=0)
		cout << base << "A" << exp << " ="  << power(base,exp)<<endl;
		else
		cout <<" Invalid Exponent Value " <<endl;
		
		return  0;
		}
		
# OUTPUT:

<img width="625" height="240" alt="image" src="https://github.com/user-attachments/assets/26fb28e5-2940-4407-9d62-f15c89e920a8" />




# QUESTION 3: Greater Finder:

#### Create a function that takes two integer values as parameters and returns the greater value of those two. Then, call that function in the main () and display the result.
#### Note: We are assuming that the values of parameters will be unique (the caller will NOT give the same value for both parameters)

## CODE:

		#include <iostream> 
		using namespace std;
		int great(int num1 , int num2){ 
		if (num1 > num2)
		return num1;
		
		else
		return num2;
		
		}
		
		
		int main(){
		int num1, num2;
		
		cout << "Number 1 = "; 
		cin >> num1; 
		cout << "Number 2 = "; 
		cin >> num2;
		if (num1 != num2)
		cout <<"Greater number is " <<great(num1,num2);
		else
		
		return 0;
		}


# OUTPUT:
 
<img width="613" height="209" alt="image" src="https://github.com/user-attachments/assets/7a8c618a-02ca-46ab-a306-fec4f9ca5fc2" />




# QUESTION 4: Factorial:

#### Create a function that takes one integer value as a parameter and then returns the Factorial of a non­ negative integer. 

## CODE:

		#include <iostream> 
		using namespace std;
		int factorial(int n){
		int result = 1 ;
		for( int i= n; i>=1; i--){ 
		result *= i,
		}
		return result;
		}
		
		int main(){
		int num;
		cout <<"Enter Number: ";
		cin >> num;
		      cout << num << "! is equal to " << factorial(num); 
		return 0;
		}


# OUTPUT:

<img width="629" height="183" alt="image" src="https://github.com/user-attachments/assets/b8575d8c-abe2-4ca2-a954-8742a03ce2f7" />




# QUESTION 5: Even or Odd:
#### Create a function that takes one integer value as a parameter and then return the word Even (if that number is an even number) or Odd (if the value is odd).

## CODE:

		#include <iostream> 
		using namespace std; 
		string evenOdd(int a){
		if(a%2 == 0)
		return "Even";
		
		else
		return "Odd";
		}
		int main(){
		int num;
		cout << "Enter Number:"; 
		cin >> num;
		cout << num << "is" << evenOdd(num);
		return  0;
		}



# OUTPUT:

<img width="610" height="191" alt="image" src="https://github.com/user-attachments/assets/199120b7-8a3b-44cd-872c-15b2f285da2e" />




# QUESTION 6: Number is Prime or Not:

#### Create a function that takes an integer value as a parameter and returns a boolean value (true or false) depending on whether the parameter value is prime or not. If that value is prime, the function should return true; otherwise, it should return false.
#### In the end, call that function in the main () function by passing a value taken as input from the user, and depending on the returned value, print whether the number is prime or not.


## CODE:

		#include <iostream> 
		using namespace std;
		
		bool primebool(int a){
		int i;
		for(i = 2; i <= a; i++){
		if(a % i == 0) 
		break;
		}
		if(a == i)
		return true;
		
		else
		return false;
		}
		
		int main(){
		int num;
		cout << "Enter the Number to check it is prime or not: "; 
		cin >> num;
		if( primebool(num) == true)
		cout << "The Number is prime";
		
		else
		cout << "The number is not Prime";
		return  0;
		}


# OUTPUT:

<img width="641" height="143" alt="image" src="https://github.com/user-attachments/assets/1fb2873e-fddd-4947-a820-12b8818d13ee" />




# QUESTION 7:

#### Write a C++ program that defines a function display to show the information. The program should take four user-defined values, i.e., int id, string name, double salary, and char gender.



## CODE:

		#include <iostream> 
		#include <string> 
		using namespace std;
		void display(int id, string name, double salary, char gender) { 
		cout << "\nEmployee Information" << endl;
		cout << "ID: " << id << endl;
		cout << "Name: " << name << endl; 
		cout << "Salary: " << salary<< endl; 
		cout << "Gender: " << gender<< endl;
		}
		
		int main() { 
		int id;
		string name; 
		double salary; 
		char gender;
		cout << "Enter ID:"; 
		cin >> id;
		cout << "Enter Name: "; 
		fflush(stdin); 
		getline(cin, name);
		cout << "Enter Salary: ";
		cin >> salary;
		cout << "Enter Gender (M/F): "; 
		cin >> gender;
		display(id, name, salary, gender); 
		return 0;
		}

# OUTPUT:

<img width="665" height="348" alt="image" src="https://github.com/user-attachments/assets/17365721-e7a7-4c67-b047-86e10c1dab03" />




# QUESTION 8: Percentage Calculator:

#### Create a function that computes the percentage of a student. The function should take two values (obtained marks and total marks) as parameters and return the percentage.

## CODE:

		#include <iostream> 
		#include<iomanip> 
		using namespace std;
		
		double per(int obtM, int totM){ 
		double result;
		cout << fixed << setprecision(2); 
		result = float (obtM) /totM* 100;
		return result;
		}
		
		int main(){
		int obt, total;
		cout << "Enter obtained Marks:"; 
		cin >> obt;
		cout << "Enter Total Marks: "; 
		cin >> total;
		      cout << "The Percentage is: " << per(obt,total) << "%" << endl; 
		return 0;
		}




# OUTPUT:

<img width="615" height="197" alt="image" src="https://github.com/user-attachments/assets/6294d9c9-4f00-4dac-814c-7e759c531c93" />



# QUESTION 9: Grade Calculator:

#### Create a function that takes the percentage as a parameter and returns the grade (A, B, C, or F). The rules for calculating the grade are:

##### i. If the  percentage is between 80 and 100 (inclusive), the grade will be A
##### ii. If the  percentage is between 70 and 79, the grade should be B
##### iii. If the  percentage is between 60 and 69, the function should return the grade C
##### iv. If the percentage is less than 60, the grade will be F


## CODE:

		#include <iostream> 
		#include <iomanip> 
		using namespace std; 
		char grade(double a){
		char result;
		int b = a;
		if(b >= 80 && b <= 100)
		result = 'A';
		else if(b >= 70 && b <= 79) 
		result='B';
		else if(b>=60 && b<=69) 
		result='C';
		else if(b<60)
		      result='F'; 
		return result;
		}
		int main()
		{
		double per;
		cout << "Enter percentage: "; 
		cin >> per;
		cout << "The Grade is : " << grade(per) << endl;
		return 0;
		}




# OUTPUT:

<img width="643" height="213" alt="image" src="https://github.com/user-attachments/assets/d3fe7b11-adc8-40b4-a8e0-48b27510aab8" />



# QUESTION 10:

#### Create a user-defined function that takes on parameter range and returns the sum of all positive integers up to that range. 



## CODE:

		#include <iostream> 
		using namespace std; 
		int sum(int n){
		int result;
		for(int i=1 ; i<=n; i++){
		result += i;
		}
		return result;
		}
		int main(){
		int num;
		cout << "Enter the range upto which you find the sum : "; 
		cin >> num;
		      cout << "The sum of all " << num << " positive integers is: " << sum(num); 
		return 0;
		}


# OUTPUT:

<img width="618" height="151" alt="image" src="https://github.com/user-attachments/assets/0262ed04-89a4-411d-92fb-64d69c3dc868" />




# QUESTION 11:

#### Create a function calculateArea that calculates the area of different shapes (circle, rectangle, and triangle) using function overloading.
### Requirements:
##### • Circle: double calculateArea(double radius) - takes one argument (radius) and returns the area of a circle.
##### • Rectangle: double calculateArea(double length, double width) - takes two arguments (length and width) and returns the area of a rectangle.
##### • Triangle: double calculateArea(float base, float height) - takes two arguments (base and height) and returns the area of a triangle.


## CODE:

		#include <iostream> 
		using namespace std;
		
		double calculateArea(double radius) { 
		return 22.0/7 *radius* radius;
		}
		double calculateArea(double length, double width) { 
		return length * width;
		}
		double calculateArea(float base, float height) { 
		return O.5f * base * height;
		}
		int main() {
		double radius, length, width; 
		float base, height;
		
		cout << "Enter radius of circle:"; 
		cin >> radius;
		cout << "Area of Circle=" << calculateArea(radius) << endl;
		
		cout << "\nEnter length and width of rectangle:"; 
		cin >> length >> width;
		cout << "Area of Rectangle = " << calculateArea(length, width) << endl;
		
		cout << "\nEnter base and height of triangle:"; 
		cin >> base >> height;
		cout << "Area of Triangle = " << calculateArea(base, height) << endl;
		return  0;
		}


# OUTPUT:

<img width="481" height="224" alt="image" src="https://github.com/user-attachments/assets/9167bcea-053a-4a06-8de6-3063c14dcfec" />



# QUESTION 12:

#### Create an overloaded displaylnfo function that can take different numbers and types of arguments to display information about a person.
### Requirements:
##### • void displaylnfo(string name) - prints "Name: [name]".
##### • void displaylnfo(int age) - prints "Age: [age]".
##### • void displaylnfo(string name, int age) - prints "Name: [name], Age: [age]".

## CODE:

		#include <iostream> 
		using namespace std;
		
		void displaInfo(string name) {
		cout << "Name: " << name << endl;
		}
		
		void displayInfo(int age) {
		cout << "Age: " << age << endl;
		}
		
		void displayInfo(string name, int age) {
		cout << "Name: " << name << ", Age: " << age  << endl;
		}
		
		int main() { 
		string name; 
		int age;
		cout << "Enter name: ";
		getline(cin, name); 
		cout << "Enter age: ";
		cin >> age;
		cout << "\nDisplay Data" << endl; 
		displayInfo(name); 
		displayInfo(age); 
		displayInfo(name, age);
		return  0;
		}


# OUTPUT:

<img width="509" height="357" alt="image" src="https://github.com/user-attachments/assets/2cfd4978-e808-4db4-b18a-fda685c00374" />



