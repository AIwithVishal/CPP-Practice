## Prem Vishal

# QUESTION 1:

#### Write a C++ program that should ask a user to input an integer number and then displays/prints its table.


## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int num;
    cout << "Enter any number to print its table: "; 
    cin >> num;
    for (int i=1 ; i<=10 ; i++ ){
    cout << num << "x" << i << " = " << (num*i) <<endl;
    }
    return  0;
    }


# OUTPUT:

<img width="832" height="570" alt="image" src="https://github.com/user-attachments/assets/4932d50c-2b4b-4f37-aec1-db701347fd35" />



# QUESTION 2:
#### Write a program that ask user to input the start andthe End of the series. Then it prints whole, natural, Even and odd numbers between these ranges. 



## CODE:

    #include <iostream> 
    using namespace std;
    int main(){
    int start, end;
    cout <<"Enter Starting Number of Series: "; 
    cin >> start;
    cout <<"Enter Ending Number of Series: "; 
    cin>>end;
    
    cout <<"Whole  Numbers: ";
    for (int i=start ; i<=end ; i++){ 
    if (i>=0)
    cout << i <<" ";
    }
    
    cout <<"\nNatural Numbers: ";
    for (int i=start ; i<=end ; i++){ 
    if (i>=l)
    cout << i <<" ";
    }
    
    cout <<"\nOdd Numbers: ";
    for (int i=start ; i<=end ; i++){ 
    if( i%2 == 1)
    cout << i <<" ";
    }
    
    cout << "\nEven Numbers: ";
    for (int i=start ; i<=end ;i ++){ 
    if( i%2 == 0)
    cout << i << " ";
    }
    return  0;
    }


# OUTPUT:

<img width="1434" height="629" alt="image" src="https://github.com/user-attachments/assets/3173cc34-55be-4205-9eff-3acc5bb1046b" />



# QUESTION 3:

#### Write a program that ask user to input the start andthe End of the series. Then it prints whole, natural, Even and odd numbers between these ranges but in reverse order. 






## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int start, end;
    cout <<"Enter Starting Number of Series:"; 
    cin >> start;
    cout <<"Enter Ending Number of Series: "; 
    cin >> end;
    
    cout <<"Whole  Numbers: ";
    for (int i=end ; i>=start ; i--){ i
    f (i>=0)
    cout << i<<" ";
    }
    
    cout <<"\nNatural Numbers:"; 
    for (int i=end ; i>=start ; i--){
    if (i>=l)
    cout << i <<" ";
    }
    
    cout <<"\nOdd Numbers: ";
    for (int i=end ; i>=start ; i--){ 
    if( i%2 == 1)
    cout << i<<" ";
    }
    
    cout <<"\nEven Numbers: ";
    for (int i=end ; i>=start ; i--){ 
    if( i%2 == 0)
    cout << i <<" ";
    }
    return  0;
    }


# OUTPUT:

<img width="887" height="289" alt="image" src="https://github.com/user-attachments/assets/db47df26-b598-4704-9bfe-6760df23ed7e" />



# QUESTION 4:

#### Write a C++ program that should ask the user to input the final range up to which the loop should run and then prints ONLY the	multiples of 5 (fully divided by 5 only), as



## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int range;
    cout <<"Enter the range upto which the loop should run: "; 
    cin >> range;
    for (int i=1; i<=range; i++){ 
    if( i%5 == 0)
    cout << i <<endl;
    }
    return  0;
    }
 

# OUTPUT:

<img width="778" height="457" alt="image" src="https://github.com/user-attachments/assets/52bbd84c-a69d-41fb-aea6-267d0a15807b" />



# QUESTION 5:
#### Write program using a for loop to print a series of 10 numbers as shown below:



## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int sum=0;
    for (int i=1 ; i<=lO ; i++){ 
    sum+=i;
    cout << sum<<" ";
    }
    return  0;
    }




## OUTPUT:

<img width="851" height="223" alt="image" src="https://github.com/user-attachments/assets/edbae694-f7a2-4678-bbf8-93b45429ae2d" />



# QUESTION 6:
#### Write a C++ program that asks a user to input the range (final value) up to which the loop should run and then for each number in that range, it should tell whether the light is off or light is on. 

## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int range;
    cout <<"Enter the range upto which loop should run: "; 
    cin >> range;
    for (int i=1 ; i<=range ; i++){ 
    if ( i%2 == 1)
    cout << i <<" -> Light is OFF" <<endl;
    
    else
    cout<<i<<" -> Light is ON"<<endl;}
    
    return  0;
    }

# OUTPUT:

<img width="655" height="335" alt="image" src="https://github.com/user-attachments/assets/b151b1e8-03f6-47a4-a415-5ed437f948ed" />



# QUESTION 7:
#### Using loop, write a C++ program that displays a series of alphabets in ascending order from 'A to 'Z' and then in descending order from 'Z' to 'A'.

## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    char ch;
    
    cout <<"Alphabets in Ascending Order" <<endl; 
    for (ch='A'; ch<='Z'; ch++){
    cout << ch << " ";
    }
    
    cout <<"\n\nAlphabets in Descending Order" << endl; 
    for (ch='Z'; ch>='A'; ch--){
    cout << ch << " ";
    }
    return  0;
    }

# OUTPUT:

<img width="829" height="209" alt="image" src="https://github.com/user-attachments/assets/dbfbacd5-31a5-449f-b595-fa517f660120" />



# QUESTION 8:
#### Modify your program in the previous part so that the program will display consonants only, no vowels.

## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    char ch;
    cout <<"Consonants in Ascending Order" <<endl; 
    for (ch='A'; ch<='Z'; ch++){
    if(!( ch=='A' || ch=='E' || ch=='I' || ch=='O'|| ch=='U'))
    cout << ch <<" ";
    }
    
    cout << "\n \n Consonants in Descending Order" << endl; 
    for (ch='Z'; ch>='A'; ch--){
    if(!( ch=='A' || ch=='E' || ch=='I' || ch=='O'|| ch=='U'))
    cout << ch <<" ";
    }
    return  0;
    }

# OUTPUT:

<img width="919" height="238" alt="image" src="https://github.com/user-attachments/assets/d183c57d-d784-4f29-949c-72d411ed95a8" />



# QUESTION 9:
#### The Fibonacci sequence is a series where the next term is the sum of the previous two terms. The first two terms of the Fibonacci sequence are O and	1. The	series is as follows:
#### 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, ...
#### Write a C++ program (using loop) to print the 10 numbers of the Fibonacci series as shown above.

## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int term1 = 0, term2=1 , next_term; 
    cout << term1 <<" " << term2;
    
    for (int i=0 ; i<8 ; i++ ){
    next_term = terml + term2; 
    term1 = term2;
    term2 = next_term; 
    cout << " " << next_term;
    }
    return  0;
    }


# OUTPUT:


<img width="575" height="82" alt="image" src="https://github.com/user-attachments/assets/f455f555-ebc6-46bf-ae46-e2bb8f63e3b4" />



# QUESTION 10:

#### Write a program to ask the user to input n_courses (Total Courses), then iterate loop n_courses
time and ask user marks in each course and perform the following tasks:

##### a) Make sure n_courses is between (3 to 8)
##### b) Calculate the average of all course marks.
##### c) Calculate the total percentage of all courses.
##### d) Tell the user whether she/he is PASS/FAIL,      FAIL	less than 60, and otherwise PASS.




## CODE:

    #include <iostream> 
    using namespace std;
    int main(){ 
    int n_courses;
    int marks, sum=O; 
    float avg, per;
    
    cout << "Enter the number of courses (between 3 and 8): "; 
    cin >> n_courses;
    if (n_courses > 3 && n_courses < 8){
    for (int i=1 ; i<=n_courses ; i++){
    cout << "Enter marks for course " << i << ": "; 
    cin >> marks;
    sum+=marks;
    }
    avg = (float) sum/ n_courses;
    per =  (float) sum/(n_courses*100)*100;  
    cout << "Average Marks: " << avg <<endl; 
    cout <<"Total Percentage: "<< per << "%" <<endl; 
    if (per<60)
    cout<<"Result:  FAIL";
    else
    cout<<"Result:  PASS";
    }
    else
    
    return 0;
    }


# OUTPUT:


<img width="785" height="327" alt="image" src="https://github.com/user-attachments/assets/12b4903a-972a-4daa-aaa3-d35b4dc61dba" />



# QUESTION 11:
#### Write a program to output the N terms of HARMONIC  series and their SUM.


## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    float i,n, sum=0;
    
    cout << "Enter the Number of terms: "; 
    cin >> n;
    
    cout << "Harmonic Series: "; 
    for (i=1 ; i<=n ; i++ ){
    cout << "1/" << i;
    if (i<n)
          cout<<" + "; 
      sum+= (1/i);
    }
    cout << "\nTotal Sum is: " << sum;
    
    return  0;
    }


# OUTPUT:


<img width="944" height="147" alt="image" src="https://github.com/user-attachments/assets/1a363980-35f3-4da3-b0da-392592820b32" />



# QUESTION 12:
#### Write a program to output the N terms of HARMONIC  series and their SUM.




## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int i;
    float n, sum = 0;
    
    cout << "Enter the Number of terms: "; 
    cin >> n;
    
    cout << "Harmonic Series: "; 
    for (i=1 ; i<=n ; i++ ){
    cout << "1/" << i;
    if (i<n)
    if(i%2==0)
    cout << " + ";
    else
    cout << " - ";
    if(i%2==0)
    sum-= (1.0/i);
    
    else
    
    }
    
    sum+= (1.0/i);
    
    cout << " \nTotal Sum is: " << sum;
    
    return 0;
    }


# Output:

<img width="966" height="141" alt="image" src="https://github.com/user-attachments/assets/09bf9bc3-c481-4b03-ae41-f8bbfac7090d" />


