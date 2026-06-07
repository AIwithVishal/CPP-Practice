## Prem Vishal

# EXERCISES (PART: A) IF/ELSE AND NESTED IF ELSE


# QUESTION 1:
#### Write a program that should ask the user to input his/her marks of one subject (out of 100). Then, it should tell the CGPA according to his/her marks. Details/rules of the CGPA are given below:


## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int a;
    cout<<"Enter your Marks: "; 
    cin >> a;
    if (a> = 93 && a <= 100){
           cout<< "Your CGPA is 4.00";
    } else if ( a>=87 && a<=92) {
    	cout<< "Your CGPA is 3.67 ";
    } else if ( a>=82 && a<=86) {
           cout<< "Your CGPA is 3.33";
    } else if ( a>=77 && a<=81) {
    	cout<< "Your CGPA is 3.00";
    } else if ( a>=72 && a<=76) {
           cout<< "Your CGPA is 2.67";
    } else if ( a>=68 && a<=71) {
    	cout<< "Your CGPA IS 2.30";
    } else if ( a>=64 && a<=67) {
    	cout<< "Your CGPA IS 2.00";
    } else if ( a>=60 && a<=63) {
    	cout<< "Your CGPA IS 1.67";
    } else if ( a>=0 && a<=59) {
    	cout<< "Your CGPA IS 0.00";
    } else{
    	cout<< "ENTER VALID MARKS";
    }
    return 0;
    }
    

# OUTPUT:

<img width="908" height="252" alt="image" src="https://github.com/user-attachments/assets/f4944557-7ed7-4ac2-988f-909695287731" />



# QUESTION 2:

#### Write the program where you ask the user to input his/her marks for five subjects and calculated his/her obtained marks and percentage. So, after calculating the percentage, you should also tell his/her grade according to the rules given below:
#### Percentage

Grade
90 (or more) --> A1
80 to 89     --> A
70 to 79     --> B
60 to 69     --> C
Less than 60 --> F


## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int s1, s2, s3, s4, s5, obt; 
    float percentage;
    cout<<"Enter Marks of Subject 1 = "; 
    cin>>s1;
    cout<<"Enter Marks of Subject 2 = "; 
    cin>>s2;
    cout<<"Enter Marks of Subject 3 = ";
    cin>>s3;
    cout<<"Enter Marks of Subject 4 = "; 
    cin>>s4;
    cout<<"Enter Marks of Subject 5 = "; 
    cin>>s5;
    obt = s1+ s2 + s3 + s4 + s5; 
    percentage=   float (obt)/500*100;
    cout<<"Obtained Marks = " << obt <<endl;
    cout<<"Percentage = " << percentage << endl; 
    cout<<"Grade = ";
    if (percentage>=90){
    cout<<"A1";
    } else if (percentage>=80 && percentage<=89){ 
    cout< < "A";
    } else if (percentage>=70 && percentage<=79){ 
    cout<<"B";
    } else if (percentage>=60 && percentage<=69){ 
    cout<<"C";
    } else
    
    cout<<"F";
    
    return 0;
    }

# OUTPUT:

<img width="893" height="363" alt="image" src="https://github.com/user-attachments/assets/ab071291-72a5-4909-be21-e43f3f0b8814" />


# QUESTION 3:

#### Write a program that prompts the user to enter a vehicle's speed and the speed limit. Use the conditional statement to determine and display whether the vehicle is within the speed limit or if it's speeding. If it's speeding, calculate and display the fine amount as follows: $10 for every 5 mph (mile per hour) over the limit.

## CODE:
    #include <iostream>  
    using namespace std; int main(){
    int speed, unit, extra_sp, extra_ch, sp_limit;
    cout<< "Speed limit= "; 
    cin >> sp_limit; 
    cout << "Speed = "; 
    cin >> speed; 
    if(speed > sp_limit){
    extra_sp = speed - sp_limit; 
    unit = extra_sp / 5; 
    extra_ch = unit*lO;
    cout<<"fine is $" << extra_ch;
    }
    else if(speed <O){
    cout<<"lnvalid Speed!";
    
    }
    else {
    
    }
    return  0;
    }



# OUTPUT:

<img width="1120" height="335" alt="image" src="https://github.com/user-attachments/assets/8614a2a4-f20f-4b6b-aa9f-4f9e17160381" />



# QUESTION 4:
#### Write a program that prompts the user to input a number. The program should then output the number and a message saying whether the number is positive, negative, or zero.


## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    float num;
    cout<<"Enter Number="; 
    cin >> num;
    cout<<"The entered Number: " <<num; 
    if (num>O){
    cout<<" is postive number.";
    } else if (num<O)
    cout<<" is negative number."; 
    else if (num==O)
    cout<<" is Zero.";
    return  0;
    }




# OUTPUT:

<img width="1127" height="332" alt="image" src="https://github.com/user-attachments/assets/638316ef-722c-4f5e-8ada-4106f1bbfed1" />



# QUESTION 5:

#### Write a program that takes an integer between 1 and 7 as input, where 1 represents Sunday, 2 represents Monday, and so on. Use appropriate control structure display the corresponding day of the week as a string (e.g., "Sunday," "Monday," etc.).

## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int day;
    cout<<"Enter Day Number= "; 
    cin >> day;
    if (day == 1)
          cout<<"Sunday"; 
    else if (day== 2)
    cout<<"Monday";
    else if (day== 3)
          cout<<"Tuesday"; 
    else if (day== 4)
    cout<<"Wednesday";
    else if (day== 5)
          cout<<"Thrusday"; 
    else if (day== 6)
    cout<<"Friday";
    else if (day == 7)
    cout<<"Saturday";
    
    else
    
    return  O;
    }


# OUTPUT:

<img width="1186" height="282" alt="image" src="https://github.com/user-attachments/assets/e070cb9a-1ed1-4472-827e-454a7ca26834" />





# QUESTION 6:

#### Write a C++ program that asks the user to input two numbers and tell

a) if the first number is greater than the second number
b) if the second number is greater than the first one
c) or both numbers are equal



## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    float  numl, num2;
    cout<<"Enter Number 1 = ";
    cin>>numl;
    cout<<"Enter 3Number 2 = ";
    cin>>num2;
    if (numl>num2)
    cout<<numl <<" is greater than "<< num2; 
    else if (numl < num2)
    cout<< num2<<" is greater than "<< num1;
    else
          cout<< numl <<" is equal to "<< num2; 
    return 0;
    }


# OUTPUT:

<img width="1124" height="407" alt="image" src="https://github.com/user-attachments/assets/533cf82c-170a-4fc2-88e3-f40a8215eba3" />




# QUESTION 7:
#### Write a C++ program that asks a user to input three numbers and tell which one is the largest of them. See the sample outputs below:



## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int a,b,c;
    cout<<"Enter first number: "; 
    cin>>a;
    cout<<"Enter second number: "; 
    cin>>b;
    cout<<"Enter third number: "; 
    cin>>c;
    if (a >= b && a >= c)
    cout << "first number is greatest"; 
    else if (b > a && b >= c) 
    cout<<"second number is greatest"; 
    else if (c > a && c > b)
    cout<<"third number is greatest";
    else if (b == a && a == c) 
    cout<<"All are equal";
    return  0;
    }


# OUTPUT:

<img width="1132" height="453" alt="image" src="https://github.com/user-attachments/assets/e5df9c1a-f67a-43d0-a27b-6c2a4dffd625" />



# QUESTION 8:
#### Write a C++ program that asks a user to input two numbers and then the operator (+ or - or* or/	etc.) to show which operation is to be performed on those two numbers. 



## CODE:

    #include <iostream> 
    #include <cstdlib> 
    using namespace std; 
    int main(){
    float a,b;
    char op;
    cout<< "Enter first number: "; 
    cin >> a;
    cout<< "Enter second number: "; 
    cin >> b;
    cout<< "Now enter any of the operators (+, -, *, /): "; 
    cin >> op;
    if (op == '+')
    cout <<"Operator was plus and the result is " << (a+b ); 
    else if (op == '*')
    cout<< "Operator was multiplication and the result is " << (a*b); 
    else if (op == '-')
    cout<<" Operator was subtraction and the result is " << (a-b); 
    else if (op == '/')
    cout<<" Operator was division and the result is " << (a/b);
    else
    cout<<"Invalid operator";
    return  0;
    }


# OUTPUT:

<img width="1150" height="411" alt="image" src="https://github.com/user-attachments/assets/3b5e672d-1842-4fce-aa74-ea834c6379d8" />



# QUESTION 9:
#### Write a program to calculate the electricity bill based on the following criteria, User will input the number of units.
• Unit price 1-200 units	25 Rs.
• Unit price 201-300 units	30 Rs.
• Unit price 301-1000 units	SO Rs.
• Unit price greater than 1000 units	60 Rs.

## CODE:
    #include <iostream> 
    using namespace std;
    int main() {
    int unit, bill = 0;
    cout<< "Enter the number of units: "; 
    cin >> unit;
    
    if (unit <= 200 && unit >= 0) 
    bill = unit*25;
    else if (unit <= 300)
      bill= (200*25) + ( (unit-200)*30 ); 
    else if (unit <= lOOO)
    bill=  (200*25) + (100*30)+ ( (unit-300) *50);
    else
    bill= (200*25) + (100*30) + (700*SO) + ( (unit-1000) *60);
    
    cout << "Total electricity bill price: " << bill << " Rs" <<endl;
    
    return  0;
    }

# Output:

<img width="1150" height="351" alt="image" src="https://github.com/user-attachments/assets/9d81606f-ac96-482b-8052-5b1b14cdb685" />




# QUESTION 10:

#### Write a program that asks the frequency of color and print the corresponding color as given in the table below:

Frequency Color:
Less than 508 --> Red
508-525       --> Yellow
526-605       --> Green
606-668       --> Blue
More than 668 --> Violet

## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int frequency;
    cout << "Enter frequencey of colour: "; 
    cin >> frequency;
    if (frequency < 508)
    cout << "Red";
    else if (frequency >= 508 && frequency <= 525) 
    cout << "Yellow";
    else if (frequency >= 526 && frequency <= 605) 
    cout << "Green";
    else if (frequency >= 606 && frequency <= 668) 
    cout<<"Blue";
    else
    
    cout<<"Violet";
    
    return 0;
    }


# OUTPUT:

<img width="1131" height="348" alt="image" src="https://github.com/user-attachments/assets/7d98c4e7-0713-4699-96dc-ce9379d58da2" />



# EXERCISES (PART: B) SWITCH STATEMENT


# QUESTION 1:
 
#### Write a program that asks the user to input two numbers and an operator (+, -,*, or/), and then perform the operation (addition, subtraction, multiplication, or division) on the two entered numbers according to the operator input by the user. If the  entered operator is not from these four operators, the program should display an error message saying that the entered operator is invalid.

## CODE:

    #include <iostream> 
    #include <string> 
    using namespace std; 
    int main(){
    int a , b; 
    char op;
    cout << "ENTER FIRST NUMBER: ";
    cin >> a;
    cout << "ENTER SECOND NUMBER: ";
    cin >> b;
    cout << "ENTER ANY OF THE OPERATORS ( +, - , *, /):	";
    cin >> op;
    switch(op){
    case '+' :
    cout << "Operatar was plus and the result is: " << a+b; 
    break;
    case '-' :
    cout << "Operatar was subtaction and the result is: " << a-b; 
    break;
    case '*' :
    cout << "Operatar was multiplication and the result is: " << a*b; 
    break;
    case '/' :
    cout << "Operatar was division and the result is: " << a/b; 
    break;
    default:
    cout< < "Invalid operator";
    }
    return 0;
    }


# OUTPUT:

<img width="1155" height="384" alt="image" src="https://github.com/user-attachments/assets/01245b0a-88b5-4444-b99b-2b2c4f87ed66" />



# QUESTION 2:

#### Write a program that should ask the user to input a month number (from 1 to 12) and then display the respective month name in words (like January for 1, February for 2 and so on). If the user inputs value other than numbers from 1 to 12, the program should display a message saying that it is an invalid month number.

## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int month;
    cout<<" Month Number: "; 
    cin >> month; 
    switch(month){
    case 1:
    	cout<<"January"; 
    break;
    
    
    case 2:
    	cout<<"Febrauary"; 
    break;
    
    case 3:
    	cout<<"March"; 
    break;
    
    case 4:
    	cout< <''April"; 
    break;
    
    case 5:
    	cout<<"May"; 
    break;
    
    case 6:
    
    	cout<<"June"; 
    break;
    
    case 7:
    	cout<<"July"; 
    break;
    
    case 8:
    	cout<<''August"; 
    break;
    
    case 9:
    
    	cout<<"September"; 
    break;
    
    case 10:
    	cout<<"October"; 
    break;
    
    case 11:
    	cout<<"November"; 
    break;
    case 12:
    	cout<<"December"; 
    break;
    default:
    	cout<<"lnvalid Month Number";
    
    }
    return  0;
    }


# OUTPUT:


<img width="1147" height="289" alt="image" src="https://github.com/user-attachments/assets/58cb186e-9983-41d8-b9c4-341d0553e287" />





# QUESTION 3:
#### Write a program that ask the user to input a month (from 1 to 12) and then display which season currently it is. The season should be displayed as per the following rules

•If the
month number is 12 or 1 or 2, then it is the Winter season
•If the
month number is 3 or 4, then it is the Spring season
•If the
month number is 5 or 6 or 7 or 8 or 9, then it is the summer season
•If the
month number is 10 or 11, then it is the Autumn season

## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int month;
    cout << "Month Number: "; 
    cin >> month; 
    switch(month){
    case 12:
    case 1:
    case 2:
    	cout<<"Winter Season"; 
    break;
    
    case 3:
    case 4:
    	cout<<"Spring Season"; 
    break;
    
    case 5:
    case 6:
    case 7:
    case 8:
    case 9:
    
    	cout<<"Summer Season"; 
    break;
    case 10:
    case 11:
    	cout<<''Autumn Season";
     break;
    default:
    	cout<<"Invalid Month Number";
    
    
    }
    return 0;
    }


# OUTPUT:


<img width="1131" height="265" alt="image" src="https://github.com/user-attachments/assets/d50c9f1d-202b-4b86-8e87-b165b0eafcb0" />



# QUESTION 4:
#### Write a program that should ask the user to input an alphabet character (small or capital) and tell if it is a vowel or a consonant.


## CODE:
    #include <iostream> 
    using namespace std;
    int main(){
    char ch;
    cout<<"Enter Alphabet: "; 
    cin>>ch;
    bool b = (ch >= 'a' && ch <='z') || ( ch >= 'A' && ch<='Z'); 
    switch(b){
    case 1:
    switch(ch){
    case 'a': case 'e': case 'i': case 'o': case 'u':
    case 'A': case 'E': case 'I': case 'O': case 'U': 
    	cout << "The alphabet is vowel" <<endl; 
    break;
    default:
    	cout<<"The alphabet is consonant"<<endl;
    
    }
    break; 
    case 0:
    	cout<<"lnvalid Input"<<endl;
    }
    return  0;
    }



# OUTPUT:


<img width="1220" height="268" alt="image" src="https://github.com/user-attachments/assets/43d0dc80-1a81-424d-afb6-adf7a3e35ea2" />



# QUESTION 5:

#### Write a program that should ask the user to input an integer number and print whether it is even or odd.


## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int num , result;
    cout << "Enter the number: "; 
    cin >> num;
    result = num % 2 ; 
    switch(result){
    case 0:
    cout << "Number is even"; 
    break;
    case 1:
    case -1:
    cout<<"Number is odd"; 
    break;
    
    }
    return  0;
    }

# OUTPUT:

<img width="1150" height="282" alt="image" src="https://github.com/user-attachments/assets/f4cec8f9-42a9-4219-92eb-9ded80cc7809" />




