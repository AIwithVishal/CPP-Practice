### Prem Vishal
# QUESTION 1:
#### Write a program that generates the spacing word output by using setw, left, right and endl manipulators.


## CODE:
  #include <iostream>
  #include <iomanip> 
  using namespace std; 
  int main(){
  
  cout<<"Programming" <<endl
  <<setw(20) <<"Fundamentals" <<endl
  <<setw(20) <<"C++" <<endl;
  
  return  O;
  }


# OUTPUT:
<img width="1196" height="407" alt="image" src="https://github.com/user-attachments/assets/5af1d669-0f3e-4ede-aa1c-1d1ae1101383" />




# QUESTION 2:

#### Write a program to print the following shapes using the setw and endl manipulator only(Don't use and escape sequence or spaces).
Hint: setw only affects the immediately following output. It doesn't persist for subsequent outputs.

(a)
<img width="262" height="269" alt="image" src="https://github.com/user-attachments/assets/0fc21c49-ca42-455f-acaa-28e661e4088a" />



## CODE:
  #include <iostream> 
  #include <iomanip> 
  using namespace std; 
  int main(){
  
  cout << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#" 
  << endl;
  cout << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << endl;
  cout << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << endl;
  
  cout << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << endl;
  
  
  cout << "#"
  << setw(2) << "#"
  << endl;
  
  
  
  cout << "#"
  << endl;
  
  return  O;
  }


# OUTPUT:
<img width="1151" height="565" alt="image" src="https://github.com/user-attachments/assets/8818ebf1-10b3-43ca-8217-5e2779c200b2" />



(b)
<img width="1178" height="656" alt="image" src="https://github.com/user-attachments/assets/5f2db13b-3c44-40e9-96d7-e2c962a83ab1" />


## CODE:

  #include <iostream>
  #include <iomanip> 
  using namespace std;
  int main(){
  
  cout << "#" << endl;
  cout << "#" << setw(2) << "#"
  << endl;
  cout << "#" << setw(2) << "#"
  << setw(2) << "#"
  << endl;
  
  cout << "#" << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << endl;
  cout << "#" << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#" << endl;
  cout << "#" << setw(2) << "#"
  << setw(2) << "#"
  << setw(2) << "#"
  << endl;
  cout << "#" << setw(2) << "#"
  << setw(2) << "#"
  << endl;
  
  cout << "#" << setw(2) << "#"
  << endl;
  
  
  cout << "#" << endl;
  
  return  O;
  }


# OUTPUT:

<img width="204" height="312" alt="image" src="https://github.com/user-attachments/assets/544484a5-2488-4bcd-b7cb-0d698d4c96a9" />


(c)
<img width="302" height="388" alt="image" src="https://github.com/user-attachments/assets/9aa1a1d1-dab2-4edb-b019-6671a520877e" />


# CODE:
  #include <iostream> 
  #include<iomanip> 
  using namespace std; 
  int main(){
  
  cout << setw(7) << "###" <<endl;
  cout << setw(4) << "#" << setw(4)<< "#" <<endl; 
  cout << setw(3) << "#" << setw(6)<< "#" <<endl; 
  cout << setw(2) << "#" << setw(8)<< "#" <<endl;
  cout << setw(2) << "#" << setw(8)<< "#" <<endl;
  cout << setw(2) << "#" << setw(8)<< "#" <<endl; 
  cout << setw(3) << "#" << setw(6)<< "#" <<endl; 
  cout << setw(4) << "#" << setw(4)<< "#" <<endl; 
  cout << setw(7) << "###" <<endl;
  
  return  0;
  }


# OUTPUT:
<img width="1174" height="662" alt="image" src="https://github.com/user-attachments/assets/1dd080a5-131e-43b9-93b5-a261f423530c" />



(d)
<img width="273" height="373" alt="image" src="https://github.com/user-attachments/assets/0dc674be-9472-4ddc-9be7-c1bccb780e6b" />



## CODE:
  #include <iostream> 
  #include <iomanip> 
  using namespace std; 
  int main(){
  
  
  cout << setw(5) << "#"
  <<endl;
  cout << setw(4) << "#"
  << setw(2) << "#"
  << endl;
  cout << setw(3) << "#"
  << setw(4) << "#"
  << endl;
  cout << setw(2) << "#"
  << setw(6) << "#"
  << endl;
  cout << setw(1) << "#"
  << setw(8) << "#"
  << endl;
  cout << setw(2) << "#"
  << setw(6) << "#"
  << endl;
  cout << setw(3) << "#"
  << setw(4) << "#"
  << endl;
  cout << setw(4) << "#"
  << setw(2) << "#"
  << endl;
  cout << setw(5) << "#";
  
  return  0;
  }



# OUTPUT:
<img width="1147" height="614" alt="image" src="https://github.com/user-attachments/assets/88f3614f-d438-4f98-b15a-b950feb5ba2c" />


# Question 3:

#### Write a program that asks the user to input two numbers i.e., num1 and num2;
#### And the output should be formatted according to these numbers. The larger number will print the larger gap on the screen (use setw and right align).


## CODE:
  #include <iostream> 
  #include <iomanip> 
  using namespace std;
  int main(){
  
  int num1,num2; 
  cout << "Enter 1st value: "; 
  cin >> numl;
  cout<<"Enter 2nd value: "; 
  cin >> num2;
  cout << setw(numl) << numl <<"  slots" <<endl
        <<setw(num2) << num2 <<" slots" <<endl; 
   return O;
  }


# OUTPUT:

<img width="1134" height="456" alt="image" src="https://github.com/user-attachments/assets/8b946975-3861-4b0a-a48c-8e857ba89604" />




# Question 4:

#### Generate the listed items using the Manipulators only (setw(n), endl, fixed, left, etc.)
#### Hint: You may use setprecision(n), left/right, and fixed only once in a program. No need to use them again and again.



## CODE:

  #include <iostream> 
  #include <iomanip> 
  using namespace std;
  int main(){
  
  cout <<"===========================\n"; 	
  cout <<"\t  HYPER MALL\n";
  cout <<"===========================\n"; 
  
  cout << left << setw(10) << "1tems" << setw(10) << "Small"
  << setw(10) << "Medium" << setw(10) << "Large" <<  endl;
  cout << setprecision(2) << fixed
  << setw(10) << "Box" << setw(10) << 20.50 << setw(10)
  << 40.59 << setw(10) << 60.75 <<endl;
  cout << setw(10) << "Bottle" << setw(10) << 18.59 << setw(10)
  << 29.84 << setw(10) << 35.75 <<endl; 
  cout << setw(10) << "Socks" << setw(10) << 20.50 << setw(10)
  <<50.59 << setw(10) <<99.75 <<endl; 
  cout << setw(10) << "Beg" << setw(10) << 89.87 << setw(10)
  << 92.87 << setw(10) << 99.89 <<endl;
  cout<< setw(10) << "Glass" << setw(10) << 70.50 << setw(10) 
  << 80.59 << setw(10) << 90.75 <<endl;
  cout << setw(10) << "Ball" << setw(10) << 67.89 <<setw(10)
  << 78.97 << setw(10) << 98.65 <<endl; 
  cout << setw(10) <<"Diary" << setw(10) <<50.78 <<setw(10)
  <<60.50 << setw(10) << 70.45 <<endl; 
    return 0;
  }


# OUTPUT:

<img width="980" height="642" alt="image" src="https://github.com/user-attachments/assets/0f7872dd-b930-4116-9cdc-f63f629c0c7d" />



# Question 5:

## Write a program in which you create three float variables to set the price of 240.99999 for a joystick, 180.88888 for disk, and 570.77777 for keyboard. Your task is to print the prices of the above-mentioned items in the following format.
## NOTE: After decimal points, your program must print two digits.


# CODE:

  #include <iostream> 
  #include <iomanip> 
  using namespace std;
  int main(){
  
  float num1 = 240.99999, num2 = 180.88888, num3 = 570.77777;
  
  cout << "===========================\n";
  cout << "\t   TECHNO ELECTRONICS\n";
  cout << "===========================\n";
  cout << setw(8) <<"" << left << setw(8) << "Joystick"
  << setw(3) << ":" << setw(8) << setprecision(2) <<fixed
  << num1 << endl; 
  cout << setw(8)<<""<< left << setw(8) << "Disk" 
  <<setw(3) <<":" << setw(8) << setprecision(2) <<fixed
  << num2 <<endl;
  cout << setw(8) <<""<< left << setw(8) << "Keyboard"
  << setw(3) <<":"<< setw(8) << setprecision(2)<<fixed 
  << num3 <<endl;
   return 0;
  }

# OUTPUT:

<img width="1211" height="548" alt="image" src="https://github.com/user-attachments/assets/e29f2f08-059d-4f32-abaf-528080e3d9d2" />


# Question 6:

#### Write a program for the marksheet, where user should be able to enter the marks for five subjects. Then, your program should tell him/her his/her obtained marks, average marks and percentage.
#### Note: You can assume each subject to be of 100 marks. So, the total marks would become 500 for five subjects. 




## Code:

  #include <iostream> 
  #include <iomanip> 
  using namespace std;
  int main(){
  
  float CPP,ICT,OOP,Maths,Eng; 
  float obt,avg,per;
  
  cout <<"Enter marks of CPP: ";
  cin >> CPP;
  cout << "Enter marks of ICT: "; 
  cin >> ICT;
  cout << "Enter marks of OOP: ";
  cin >> OOP;
  cout <<"Enter marks of Maths: ";
  cin >> Maths;
  cout <<"Enter marks of English: ";
  cin >> Eng;
  
  obt = CPP+ICT+OOP+Maths+Eng; 
  avg = (CPP+ICT+OOP+Maths+Eng)/5; 
  per = obt/500*100;
  
  cout <<" ****************************************\n";
  cout <<"\t	MARKSHEET\n";
  cout <<" ****************************************\n";
  
  cout << left << setw(20) << "Student Name:" <<setw(10) <<"Prem Vishal" <<endl; 
  cout << left << setw(20) << "CMS ID:" << setw(10) <<"222-22-2222" << endl;
  
  cout <<"****************************************\n"; 
  cout << left << setw(15) << "SUBJECT" << setw(7) <<"MARKS"
  <<endl;
  cout <<" ****************************************\n";
  cout << setprecision(2) << fixed << showpoint
       << setw(15) << "CPP" << setw(7) << CPP << endl; 
  cout << setw(15) << "ICT" << setw(7) << ICT << endl; 
  cout << setw(15) << "OOP" << setw(7) << OOP << endl; 
  cout << setw(15) << "Maths"<< setw(7) <<Maths << endl; 
  cout << setw(15) << "English"<<setw(7)<<Eng << endl;
  
  cout <<" ****************************************\n";
  cout << setw(15) << "Obtained Marks" << setw(7) <<obt <<endl;  
  cout << setw(15) << "Average Marks" << setw(7) <<avg << endl;   
  cout << setw(15) << "Percentage" <<setw(7) << per <<"%" <<endl;     
  cout <<" ****************************************\n";
  
  return 0;
  }

# OUTPUT:

<img width="530" height="884" alt="image" src="https://github.com/user-attachments/assets/17c94939-553a-488b-80ac-20dd7efb7786" />


















