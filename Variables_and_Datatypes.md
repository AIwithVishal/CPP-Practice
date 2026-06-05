
# VARIABLES and DATATYPES

# Question 1:
#### Write a program that takes 5 values from the user:
    --> one value of String (name),
    --> one value of int (age),
    --> one value of double (salary),
    --> one value of boolean (isMarried),
    --> one value of char (grade).
#### Print each value on saparate line:

# CODE:
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







![App Screenshot](https://dummyimage.com/468x300?text=App+Screenshot+Here)

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







![App Screenshot](https://dummyimage.com/468x300?text=App+Screenshot+Here)    

