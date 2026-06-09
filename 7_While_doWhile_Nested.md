
# EXERCISES (PART: A) WHILE AND DO WHILE LOOP

# QUESTION 1:

#### Write a C++ program that should continuously ask the user to input any integer number until and unless a negative number is entered. When a negative number is entered, then the program should end and print the sum of all the entered numbers.
#### However, it should also check that large numbers (greater than 30) should not be considered for calculating the sum, like shown below:



## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int sum = 0, num; 
    do{
    cout<<"Enter a number: ";
    cin >> num; 
    if (num>30)
    cout << "The number is greater than 30 and won't be calculated.\n";
    else if(num >= 0)
    sum += num;
    }while(num>=0); 
    cout << "The sum is " << sum;
    return 0;
    }

# OUTPUT:

<img width="878" height="521" alt="image" src="https://github.com/user-attachments/assets/75f9d7cb-bdae-45ff-857d-b7ad0a988e08" />





# QUESTION 2:

#### Write a C++ program that receives the total number of integers (N) from the user. Then, the program will ask the user for N real numbers. By applying for loop, your program should find and display the largest and the lowest of the numbers. Give a proper message for invalid user input, as shown below:



## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int range;
    float low, high, num;
    cout << "How many numbers do you have? > "; 
    cin >> range;
    if (range == 0)
          cout << "Oops! You don't have any number for me to process.\n"; 
    else if(range<0)
    cout <<"Sorry, you have entered an invalid input.\n";
    
    else{
    
    
    for( int i=1 ; i<=range ; i++){
    cout << "Please enter a number_" << i <<" --> ";
    
    cin >> num; 
    if(i==1){
    low = num;
    high = num;
    }
    else{
    
    }
    
    
    if (num>high)
          high = num; 
    if (num < low)
    low = num;
    
    }
    cout <<"\nThe lowest number is " << low; 
    cout <<"\nThe highest number is "<< high; 
    cout<<endl;
    }
    
          cout<<"Thankyou."; 
    return 0;
    }


# OUTPUT:

<img width="892" height="536" alt="image" src="https://github.com/user-attachments/assets/10041ade-bdcf-42a1-8867-ebf3247cb4e6" />



# QUESTION 3:


#### Create a Guessing Game program, where you will guess a number. For now, assume any fixed number of choices as the actual number to be guessed (means, hardcode that value inside the code). Then, continuously ask the user to guess the number (I.e., input the number) unit and unless he/she guesses it correctly.
#### Display the message(s) to the user as described below:

##### • If the entered number is smaller than the actual number, then you should display a message saying the user that his/her entered number is smaller than the actual number
##### • If the entered number is greater than the actual number, then you should display a message saying the user that his/her entered number is greater than the actual number
##### • If the user guesses the number correctly (I.e., enters the actual number), then display a Congrats message, as shown below:




## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int guess = 23; 
    do{
    cout <<"Guess the number. Enter your guess: ";
    cin >> guess;
    if ( guess < 23 )
          cout << "Your guessed number is smaller than the actual number\n"; 
    else if (guess >23)
    cout << "Your guessed number is greater than the actual number\n";
    } while (guess!=23); 
    cout<<"Congrats! You guessed it";
    return  0;
    }

# OUTPUT:


<img width="883" height="410" alt="image" src="https://github.com/user-attachments/assets/91c1d9b4-61d7-4418-a4c2-a56e7e64b4db" />



# QUESTION 4:

#### Extend the Guessing Game program created above. Other rules are the same as stated in the previous part. However, in this program, the actual number's value should be fixed between 1 and 100 and the user should be allowed only five (05) attempts.
#### If the	user guesses the number within five attempts, then display a Congrats message. Otherwise, the program should end after five wrong attempts, and display a sorry message to the user and the actual number as well.

## CODE:

    #include <iostream> 
    #include <cstdlib> 
    #include <ctime> 
    using namespace std; 
    int main(){
    int i=1 , guess;
     srand(static_cast<unsigned int>(time(NULL)));
     int num = rand()%100+1;
    do{
    cout << "Guess the number. Enter your guess: "; 
    cin >> guess;
    if (guess<num)
          cout << "Your guessed number is smaller than the actual number"; 
    else if (guess>num)
    cout <<"Your guessed number is greater than the actual number";
    else if(guess == num)
    cout<<"Congrats. You guessed it"; 
    exit(0);
    cout << endl;
    1++;
    } while ( i<=5);
    cout << "Sorry you are out of chances. The actual number was " << num; 
    return 0;
    }

# OUTPUT:

<img width="849" height="494" alt="image" src="https://github.com/user-attachments/assets/8e615de8-d43d-4c36-bd4d-7b45a7e12536" />



# QUESTION 5:

#### Create a program for a simple shopping application, where a user will be shown a Menu from which he/she can select any product to purchase or enter zero (0) to exit the program.
#### When the user selects any product, then the program should ask the user to input the desired quantity of that product to be bought.

#### Finally, when the user enters a zero (0) to exit the program, then a detailed description should be shown that should include
##### • all the purchase products
##### • their quantity (for each product)
##### • the subtotal cost (of each product bought)
##### • and the total cost (of all the products)


## CODE:
    #include <iostream> 
    using namespace std; 
    int main(){
    int books, tshirts, shoes, choice, quantity, Total;
    books = shoes = tshirts = 0;
    
    do {
    
    cout <<"1: Books (Per item price= 500)\n"; 
    cout <<"2: T-Shirt (Per item price= 700)\n"; 
    cout <<"3: Shoes (Per pair price= 1000)\n"; 
    cout <<"O: Exit the program\n";
    cout <<"Enter any number to select product to buy or O to exit: "; 
    cin >> choice;
    
    switch(choice){
    case 1:
    
    cout <<"You have selected Books. Enter quantity: "; 
    cin >> quantity;
    books += quantity; 
    break;
    
    case 2:
    cout <<"You have selected T-Shirt. Enter quantity: "; 
    cin >> quantity;
    tshirts += quantity; 
    break;
    
    
    
    case 3:
    cout <<"You have selected Shoes. Enter quantity: "; 
    cin >> quantity;
    shoes += quantity; 
    break;
    
    
    
    
    case 0:
    cout <<"\nYou have bought " << books <<" Books (Price= "<<(books* 500) <<")"; 
    cout <<"\nYou have bought " << tshirts <<" T-Shirts (Price= "<<(tshirts * 700) <<")"; 
    cout <<"\nYou have bought " << shoes <<" Shoes (Price= "<<(shoes* 1000) <<")"; 
    Total = (books* 500) + (tshirts * 700) + (shoes* 1000);
    cout <<"\nTotal =" <<Total; 
    break;
    
    }
    
    } while(choice!=0);
    
    return  0;
    }

# OUTPUT:

<img width="660" height="761" alt="image" src="https://github.com/user-attachments/assets/dcb287b5-3889-4d4a-a1df-468d5b0bfddb" />



# EXERCISES (PART: B) NESTED LOOP

# QUESTION 1:
#### Using nested loops, write separate C++ programs to generate the different shapes in outputs.

# '1'

## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    
    for (int i=1 ; i<=5; i++){
    for (int j=1; j<=5 ; j++){ 
    cout << j << " ";
    }
    cout<<endl;
    
    }
    return 0;
    }

# Output:

<img width="194" height="179" alt="image" src="https://github.com/user-attachments/assets/301670db-32cc-46ae-8c2f-b6ee4abef14b" />



# '2'
## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    
    for (int i=1; i<=5; i++){
    for (int j=i; j<=4; j++){ 
    cout << " ";
    }
    for (int k=1 ; k <= i ; k++){ 
    cout << "*";
    
    return 0;
    }

    }
    cout<<endl;
    }

    
# Output:

<img width="188" height="184" alt="image" src="https://github.com/user-attachments/assets/e4d3bc7e-8564-4a7c-86bc-c5d59bfd06af" />



# '3'

## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    
    for (int i=1 ; i<=5; i++){
    for (int j=1 ; j<=i; j++){ 
    cout << "* ";
    }
    cout <<endl;
    }
    return 0;
    
  }

  
# Output:

<img width="194" height="189" alt="image" src="https://github.com/user-attachments/assets/409c3ec2-5dad-4b8c-bbd5-e90eb99874b4" />

    


# '4'

## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    
    for (int i=1; i<=5; i++){
    for (int j=i; j<=5; j++){ 
    cout << "* ";
    
    }
    cout<<endl;
    }
    
    
    return  O;
    }

# Output:

<img width="187" height="198" alt="image" src="https://github.com/user-attachments/assets/7ffe229a-ca45-4e75-b776-950b2caedebc" />



# '5'

## CODE:


    #include <iostream> 
    using namespace std; \
    int main(){
    for (int i=1 ; i<=5; i++){
    for (int j=1; j<=5-i; j++){ 
    cout << " " ;
    }
    for (int k=1 ; k<=2*i-1; k++){ 
    cout << " *";
    }
    cout << endl;
    }
    return 0;
    }

    
# Output:

<img width="319" height="191" alt="image" src="https://github.com/user-attachments/assets/b186b359-0959-4a18-a5ac-1edeaf097592" />




# QUESTION 2:

#### Write a program that computes average test scores of students. The program should first ask the user to input total number of students and then the number of test scores per student. After that, for each student, ask the user to enter test scores and compute (and display) the average test score of every student.



## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int i , j , students , subjects;
    float score, avg, sum  = 0;
    cout <<"This program averages test scores.\n"
          <<"For how many students do you have scores?"; 
    cin >> students;
    cout <<"How many test scores does each student have?"; 
    cin >> subjects;
    if(students > 1 && subjects > 1){ 
    for (i=1 ; i <=students ; i++){
    for (j=1 ; j <=subjects ; j++){
    cout <<"Enter Score " << j << " for student " << i <<": ";
    
    cin >> score;
    sum += score;
    }
    avg = sum/subjects;
    cout <<"The average score for student " << i <<" is " << avg; 
    cout <<endl << endl;
    sum = 0;
    }
    }
    else
    cout << "lnvalid Input Values";
    return  0;
    }



# OUTPUT:

<img width="964" height="700" alt="image" src="https://github.com/user-attachments/assets/da5c4cd2-7a6b-4326-8630-8df02740a22c" />



# QUESTION 3:

#### Write a program that asks the user to input an integer value that denotes the range up to which tables of number should be printed. Then, tables of all the numbers from 1 to that range value should be displayed.

## CODE:

    #include <iostream> 
    using namespace std; 
    int main(){
    int range;
    cout <<"Enter the range upto which you want to find tables: "; 
    cin >> range;
    
    for(int i=1 ; i<=range; i++){ 
    cout << "Table of " << i <<endl; 
    for(int j=1 ; j<=10 ; j++){
    cout << j <<" x " << i <<" = " << i*j <<endl;
    }
    cout << endl;
    }
    return 0;
    }


# OUTPUT:

<img width="676" height="808" alt="image" src="https://github.com/user-attachments/assets/4381c623-e854-4e93-83d6-643932a99fcf" />







