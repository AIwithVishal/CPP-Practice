
# VARIABLES and DATATYPES

# Question 1:
#### Write a program that takes 5 values from the user:
    --> one value of String (name),
    --> one value of int (age),
    --> one value of double (salary),
    --> one value of boolean (isMarried),
    --> one value of char (grade).
#### Print each value on saparate line:

## CODE:
    #include <iostream>
    using namespace std;
    int main(){
    string name;
    int age;
    double salary;
    boolean isMarried;
    char grade;

    cout << "Enter your name: ";
    getline(cin, name);
    cout << "Enter your age: ";
    cin >> age;
    cout << "Enter your salary: ";
    cin >> salary;
    cout << "Are you married? ";
    cin >> isMarried;
    cout << "Enter your grade: ";
    cin >> grade;

    cout << "Name: " << name << endl;
    cout << "Age: " << age << endl;
    cout << "Salary: "<< salary << endl;
    cout << "Married: "<< boolalpha << isMarried << endl;
    cout << "Grade: "<< grade;
        return 0;
    }

 # OUTPUT:
 <img width="922" height="484" alt="image" src="https://github.com/user-attachments/assets/be0e5d22-580f-4fa2-ba0e-ab3c4a4f309f" />






# Question 2:

#### Write a program that calculate the percentage of given obatined and total marks:

## CODE:
    #include <iostream>
    using namespace std;
    int main(){
    float obtMarks;
    float ttlMarks;
    float percent;

    cout << "Enter your obtained marks: ";
    cin >> obtMarks;
    cout << "Enter your total marks: ";
    cin >> ttlMarks;

    percent = (obtMarks/ttlMarks)*100;
    cout << "The percentage of your marks is: " <<
    percent << "%"; 
        return 0;
    }

 # OUTPUT:
 <img width="1566" height="649" alt="image" src="https://github.com/user-attachments/assets/fbb8233c-42bf-4829-a534-ba4f92122732" />



# Question 03

#### Write a program that finds the value of X by using given formula. Take value of 'm' and 'n' from user:
#### X = (m2 + n2)-2mn


## CODE:
	#include <iostream> 
	using namespace std;
	int main() { 
	int m, n, X;

	cout << "Enter value of m: "; 
	cin >> m;
	cout << "Enter value of n: ";
	cin >> n;
	
	X = (m * m + n * n) - (2 * m * n);
	
	cout << "\nValue of X =" << X << endl;
	
	
	return  O;
	}


# OUTPUT:
<img width="1222" height="492" alt="image" src="https://github.com/user-attachments/assets/65dd7840-57bf-4697-9ce0-e064f2e99bda" />



# Question 4

#### Write a program that asks the user to type character then the program will generate its ASCII value.

## CODE:

	#include <iostream> 
	using namespace std; 
	int main(){
	char a; 
	int b;
	cout << "Enter any character: ";
	Cin >> a;
	 b=a;
	  cout << "The ASCII Value of" << a << "is" << b; 
	return O;
	}


# OUTPUT:
<img width="851" height="246" alt="image" src="https://github.com/user-attachments/assets/152a9d5d-cd16-4b5a-9c64-6952e29a5f39" />


# Question 5:

#### Write a program that takes a Number (integer) input from the user and then it prints the Character associated with that ASCII. 

## CODE:

	#include <iostream> 
	using namespace std;  
	int main(){
	int num;
	cout<<"Enter any Number: "; 
	cin >> num;
	cout << "The character w.r.t " << num <<" is:"<<char(a); 
		return O;
	}

# OUTPUT:
<img width="878" height="216" alt="image" src="https://github.com/user-attachments/assets/06ee80c0-bf5b-4484-bf49-e7f60fee9261" />




# QUESTION 6:
#### Write a program that asks the user to type lowercase (small) alphabet character then the program will generate its uppercase (capital) alphabet character. 

## CODE:

	#include <iostream> 
	using namespace std; 
	int main(){
	char a;
	cout << "Enter Lowercase alphabet charachter: "; 
	cin >> a;
	cout << "The Uppercase of "<< a <<" is:" << char(a-32);
	
	return  O;
	}


# OUTPUT:

<img width="867" height="259" alt="image" src="https://github.com/user-attachments/assets/cc25d9b5-64af-47f2-b7b7-33adcafba0c9" />



# QUESTION 7:

#### Write a program that asks the user to type uppercase (capital) alphabet character then the program will generate its lowercase (small) alphabet character. 

## CODE:

	#include <iostream> 
	using namespace std; 
	int main(){
	char a;
	cout << "Enter Uppercase alphabet charachter: "; 
	cin >> a;
	cout << "The Lowercase of " << a <<" is: " << char(a+32); 
	return O;
	}


# OUTPUT:

<img width="860" height="256" alt="image" src="https://github.com/user-attachments/assets/95793237-a671-40e2-add5-07069d9c0ea8" />













