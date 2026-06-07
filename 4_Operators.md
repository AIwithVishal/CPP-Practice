Prem Vishal
# QUESTION 1:
#### Length and  breadth of a rectangle are 5 and 7 respectively. Write a program to calculate the area and perimeter of the rectangle.



# CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int len=5, width=7;
    int p=(len+width)*2; 
    int area=len*width;
    cout<<"Length is: "<<len<<endl
          <<"Breadth is: "<< width <<endl; 
    cout<<"Perimeter of Rectangle is: "<< p <<endl
    <<"Area of Rectangle is: "<<area;
    return 0;
    }

  # Output:

  <img width="1174" height="446" alt="image" src="https://github.com/user-attachments/assets/f684d4c5-be10-41ab-8f71-7ff1bf06999c" />






# QUESTION 2:
#### Write a program that inputs a six-digit integer, separates the integer into its individual digits and prints the digits vertically using modulus operator. For example, if the  user types 953647, the program should print:
                                                    7
                                                    4
                                                    6
                                                    3
                                                    5
                                                    9



## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int num;
    cout<<"Enter 6 digit number: "; 
    cin >> num;
    cout << num % l0 <<endl; 
    cout << num/10 % l0<<endl; 
    cout << num/100 % 10<<endl; 
    cout << num/1000 % 10<<endl; 
    cout << num/10000 % 10<<endl; 
    cout << num/l00000<<endl;
    return 0;
    }

# OUTPUT:
<img width="1137" height="590" alt="image" src="https://github.com/user-attachments/assets/ba165e0d-d705-4fa3-aa4a-f19631d90533" />



# QUESTION 3:
#### Write a program to convert Fahrenheit into Celsius.




## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    
    double fahrenheit , celcius;
    cout<<"Enter fahrenheit value to change into celsius: "; 
    cin >> fahrenheit;
    celcius = (double)5/9*(fahrenheit-32);
    cout<<"Celsius value is: "<< celcius ;
    
    return  0;
    }




# OUTPUT:

<img width="1139" height="341" alt="image" src="https://github.com/user-attachments/assets/5c7672d7-f687-42f2-ac68-0f7351d89409" />




# QUESTION 4:
#### Create a program to calculate and display the surface of the cylinder given the radius (r) and height (h) using the formula:
<img width="699" height="135" alt="image" src="https://github.com/user-attachments/assets/64161d0c-1e4d-4642-801a-4695b979c3b7" />







## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    
    float Surface_Area, r, h, pi=22.0 /7; 
    cout<<"Enter value of r and h: "; 
    cin >> r >> h; 
    Surface_Area= 2*pi*r*r + 2*pi*r*h;
          cout<<"Surface Area= "<< Surface_Area; 
    return 0;
    }

# OUTPUT:

<img width="1239" height="284" alt="image" src="https://github.com/user-attachments/assets/705a453e-9cb0-40bd-9626-30d51263087b" />



# QUESTION 5:
#### Write a program that takes two values for hours and minutes and then calculates total seconds
## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int hour,mint,sec;
    cout<<"Enter number of hours: "; 
    cin >> hour;
    cout <<"Enter number of minutes:"; 
    cin >> mint; 
    sec=(mint*60)+(hour*60*60); 
    cout<<"total seconds: "<< sec;
    return 0;
    
    }
# OUTPUT:

<img width="1154" height="344" alt="image" src="https://github.com/user-attachments/assets/bfb3ce05-5f6f-4827-9f0e-eb979579d4fe" />




# QUESTION 6:
#### Write a program that takes two numbers from user and checks if the two numbers are equal or not by returning true or false respectively.


## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int num1 , num2;
    bool result;
    cout<<"Enter two number: "; 
    cin >> num1 >> num2;
    result = (num1 == num2);
          cout<< boolalpha << result; 
    return 0;
    }


# Output:

<img width="1195" height="322" alt="image" src="https://github.com/user-attachments/assets/bf7326a4-5884-4958-a33d-442570a482a2" />




# QUESTION 7:
#### Write a program to enter the values of two variables 'a' and 'b' from user and then check if both the conditions 'a < 5O' and ' a < b' are true.


## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int num1 , num2;
    bool result;
    cout<<"Enter two number: "; 
    cin >> num1 >> num2;
    result= (num1 < 5O && num1 < num2);
          cout<<result; 
    return 0;
    }


# OUTPUT:

<img width="1146" height="264" alt="image" src="https://github.com/user-attachments/assets/56f82d98-a315-4e8d-a1d3-955fd45ac452" />



# QUESTION 8:
#### Write a program to enter the values of two variables 'a' and 'b' from user and then check if atleast one of the conditions 'a< 5O' and 'a < b' is true.



# CODE:
  
    #include <iostream> 
    using namespace std; 
    int main(){
    int a,b; 
    bool result;
    cout<<"Enter two number: "; 
    cin >> a >> b;
    result= (a < 5O || a < b );
          cout<< result; 
    return 0;
    }




# OUTPUT:

<img width="1136" height="281" alt="image" src="https://github.com/user-attachments/assets/063d6535-4f56-43ab-87a3-bec7552981d8" />



# QUESTION 9:
#### Implement a program that calculates the square of a number entered by the user (using assignment operator).


## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int num;
    cout<<"Enter any number: "; 
    cin >> num;
          cout<<"Square of " << num <<" is: "; 
    	num*=num·,
          cout<<num; 
    return 0;
    }


# OUTPUT:

<img width="1145" height="340" alt="image" src="https://github.com/user-attachments/assets/d7b6376e-1407-4930-8103-828ffcb94ce8" />


