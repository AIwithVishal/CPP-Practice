## Prem Vishal

# QUESTION 1:
#### Consider an integer array, the number of elements should be determined by the user. The elements are also taken as input from the user. Write a program to print sum, an average of all numbers, the smallest and largest element of an array.

## CODE:

    #include <iostream>
    using namespace std;
    int main()
    {
    	int n,a[n], sum=0,avg;
    	cout<<"Enter the number of digits you want to enter: ";
    	cin>>n;
    	for(int i=0;i<n;i++)
    	{
    	cout<<"Enter the number: ";
    	cin>>a[i];
    	sum=sum+a[i];
    	}
    	avg=sum/n;
    	
    	int largest=a[0];
    	int smallest=a[0];
    	
    	for(int i=1;i<n;i++)
    	{
    		if(a[i]<smallest)
    		smallest=a[i];
    		if(a[i]>largest)
    		largest=a[i];
    	}
    	cout<<"Sum= "<<sum<<endl;
    	cout<<"Average= "<<avg<<endl;
    	cout<<"Smallest= "<<smallest<<endl;
    	cout<<"Largest= "<<largest;
    }



# OUTPUT:

 



## QUESTION 2:
#### Take 20 integer inputs from user and print the following: 
•	Number of positive numbers 
•	Number of negative numbers 
•	Number of odd numbers 
•	Number of even numbers
•	Number of 0. 

## CODE:

    #include <iostream>
    using namespace std;
    int main()
    {
    	int a[20], odd=0,even=0, positive=0, negative=0,zero=0;
    	for(int i=0;i<20;i++)
    	{
    		cout<<"Enter number "<<i+1<<" : ";
    		cin>>a[i];
    	}
    	for(int i=0;i<20;i++)
    	{
    		if(a[i]<0)
    		negative++;
    		if(a[i]>0)
    		positive++;
    		if(a[i]==0)
    		zero++;
    		if(a[i]%2==0)
    		even++;
    		if(a[i]%2!=0)
    		odd++;
    	}
    	cout<<"Number of positive numbers: "<<positive<<endl;
    	cout<<"Number of negative numbers: "<<negative<<endl;
    	cout<<"Number of odd numbers: "<<odd<<endl;
    	cout<<"Number of even numbers: "<<even<<endl;
    	cout<<"Number of zero numbers: "<<zero<<endl;
    }

# OUTPUT:


 
# QUESTION 3:
#### Write a program that allows the user to input a series of numbers until they enter a negative number. Store these numbers in an array and then find and print the sum of all the positive numbers entered. 

# CODE:

    #include <iostream>
    using namespace std;
    int main()
    {
    	int a[100],sum=0;
    	for(int i=0;i<100;i++)
    	{
    	    cout<<"Enter a positive integer: ";
    		cin>>a[i];
    		if(a[i]>=0)
    		sum=sum+a[i];
    		if(a[i]<0)
    		{
    		cout<<"You have entered a negative number."<<endl;
    		break;}
    	}
    	cout<<"Sum= "<<sum;
    }
    
# OUTPUT:


 
# QUESTION 4:
#### Design a program that takes 5 integer inputs from the user and stores them in an array. Find and print the frequency of each unique number in the array. 

## CODE:

    #include <iostream>
    using namespace std;
    
    int main() {
        int arr[5];
        int freq[5] = {0};  
        bool counted[5] = {false}; 
    
        cout << "Enter 5 integers: ";
        for (int i = 0; i < 5; i++) {
            cin >> arr[i];
        }
    
      
        for (int i = 0; i < 5; i++) {
            if (counted[i]) 
                continue; 
    
            int count = 1; 
            for (int j = i + 1; j < 5; j++) {
                if (arr[i] == arr[j]) {
                    count++;
                    counted[j] = true; 
            }
            freq[i] = count;
        }
    }
        cout << "\nFrequency of each unique number:\n";
        for (int i = 0; i < 5; i++) {
            if (!counted[i]) {
                cout << arr[i] << " occurs " << freq[i] << " times" << endl;
            }
        }
    
    
        return 0;
    }
    
# OUTPUT:

 
# QUESTION 5:
#### Create a program that takes 10 integer inputs from the user and stores them in an array. Find and print the second smallest and second largest numbers in the array. 

## CODE:

    #include <iostream>
    using namespace std;
    
    int main() {
        int arr[10], temp;
    
        cout << "Enter 10 integers: ";
        for (int i = 0; i < 10; i++) {
            cin >> arr[i];
        }
    
        for (int i = 0; i < 9; i++) {
            for (int j = 0; j < 9 - i; j++) {
                if (arr[j] > arr[j + 1]) {
                    temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    
        cout << "\nSecond smallest number: " << arr[1] << endl;
        cout << "Second largest number: " << arr[8] << endl;
    
        return 0;
    }

# OUTPUT:


 
# QUESTION 6:
## Ask the user to enter the size of an array (N). Then, ask them to enter N integers. 
## Check if the array is sorted in ascending order and display an appropriate message. (if it’s not sorted, then sort it using the bubble sort method) 


## CODE:

    #include <iostream>
    using namespace std;
    
    int main() {
        int n;
        cout << "Enter the size of the array: ";
        cin >> n;
    
        int arr[n];
        cout << "Enter " << n << " integers: ";
        for (int i = 0; i < n; i++)
            cin >> arr[i];
    
        bool sorted = true;
        for (int i = 0; i < n - 1; i++) {
            if (arr[i] > arr[i + 1]) {
                sorted = false;
                break;
            }
        }
    
        if (sorted) {
            cout << "\nThe array is already sorted in ascending order.\n";
        } else {
            cout << "\nThe array is not sorted. Sorting using Bubble Sort...\n";
    
            for (int i = 0; i < n - 1; i++) {
                for (int j = 0; j < n - i - 1; j++) {
                    if (arr[j] > arr[j + 1]) {
                        int temp = arr[j];
                        arr[j] = arr[j + 1];
                        arr[j + 1] = temp;
                    }
                }
            }
    
            cout << "Array after sorting: ";
            for (int i = 0; i < n; i++)
                cout << arr[i] << " ";
            cout << endl;
        }
    
        return 0;
    }


# OUTPUT:


 

# QUESTION 7:  Sales Report 
#### Imagine you work for a retail company, and you are responsible for generating a sales report. You have a list of products sold, including the product name, quantity sold, and price per unit. Write a program that calculates the total revenue for each product and the overall total revenue. Format the output using setw to display the report neatly. 

## CODE:

    #include <iostream>
    #include <iomanip> 
    using namespace std;
    
    int main() {
        int n;
        cout << "Enter number of products: ";
        cin >> n;
    
        char name[20];
        int quantity;
        float price;
        float total, grandTotal = 0;
    
        cout << "\n----- SALES REPORT -----\n";
        cout << left << setw(15) << "Product"
             << right << setw(10) << "Quantity"
             << setw(15) << "Price/unit"
             << setw(15) << "Total Revenue" << endl;
        cout << "----------------------------------------------\n";
    
        for (int i = 0; i < n; i++) {
            cout << "\nEnter product name: ";
            cin >> name;
            cout << "Enter quantity sold: ";
            cin >> quantity;
            cout << "Enter price per unit: ";
            cin >> price;
    
            total = quantity * price;
            grandTotal += total;
    
            cout << left << setw(15) << name
                 << right << setw(10) << quantity
                 << setw(15) << fixed << setprecision(2) << price
                 << setw(15) << fixed << setprecision(2) << total << endl;
        }
    
        cout << "----------------------------------------------\n";
        cout << setw(40) << "Overall Total Revenue = " 
             << setw(10) << fixed << setprecision(2) << grandTotal << endl;
        cout << "----------------------------------------------\n";
    
        return 0;
    }
    
# OUTPUT:
 

# QUESTION 8: Student Enrollment 
#### Design a program that manages student enrollment in courses. The program should allow users to add students to courses and display a list of enrolled students for each course. Use loops and conditional statements to achieve this. 

## CODE:

    #include <iostream>
    using namespace std;
    
    int main() {
        int n;
        cout << "Enter number of students to enroll: ";
        cin >> n;
    
        char students[10][30];
        cout << "\nEnter names of students:\n";
        for (int i = 0; i < n; i++) {
            cout << "Student " << i + 1 << ": ";
            cin >> students[i];
        }
    
        cout << "\nList of Enrolled Students:\n";
        for (int i = 0; i < n; i++) {
            cout << i + 1 <<" . " << students[i] << endl;
        }
    
        return 0;
    }


# OUTPUT:
 


# QUESTION 9:
#### Write a C++ program that asks the user to input an N number of values in an array (means, the size of the array as well as all the values should be input by the user) and then displays those values in reverse order. 

## CODE:

    #include <iostream>
    using namespace std;
    
    int main() {
        int n;
        cout << "Enter the size of the array: ";
        cin >> n;
    
        int arr[n];
        cout << "Enter " << n << " values:\n";
        for (int i = 0; i < n; i++) {
            cin >> arr[i];
        }
    
        cout << "Array in reverse order: ";
        for (int i = n - 1; i >= 0; i--) {
            cout << arr[i] << " ";
        }
        cout << endl;
    
        return 0;
    }

# OUTPUT:
 
# QUESTION 10:
#### Write a program that gets array size and elements as input from a user and then prints only the EVEN values that are present in the array.

## CODE:

    #include <iostream>
    using namespace std;
    
    int main() {
        int n;
        cout << "Enter the size of the array: ";
        cin >> n;
    
        int arr[n];
        cout << "Enter " << n << " values:\n";
        for (int i = 0; i < n; i++) {
            cin >> arr[i];
        }
    
        cout << "Even numbers in the array: ";
        for (int i = 0; i < n; i++) {
            if (arr[i] % 2 == 0) {
                cout << arr[i] << " ";
            }
        }
        cout << endl;
    
        return 0;
    }

# OUTPUT:
 

# QUESTION 11:
#### Write a program where you should sum the elements of two same-sized arrays and the result should be saved in the third array. Then, print the values of all of the three arrays. 
#### The values of the first two arrays may be given fixed (no need to get input) but each value of the third array should be the sum of respective values from the first and the second arrays. 

## CODE:

    #include <iostream>
    using namespace std;
    
    int main() {
        int size;
        cout << "Enter size of arrays: ";
        cin >> size;
    
        int arr1[size], arr2[size], sum[size];
    
        cout << "Enter values for first array:\n";
        for (int i = 0; i < size; i++) cin >> arr1[i];
    
        cout << "Enter values for second array:\n";
        for (int i = 0; i < size; i++) cin >> arr2[i];
    
        for (int i = 0; i < size; i++) {
            sum[i] = arr1[i] + arr2[i];
        }
    
        cout << "\nFirst array: ";
        for (int i = 0; i < size; i++) cout << arr1[i] << " ";
        cout << "\nSecond array: ";
        for (int i = 0; i < size; i++) cout << arr2[i] << " ";
        cout << "\nSum array: ";
        for (int i = 0; i < size; i++) cout << sum[i] << " ";
        cout << endl;
    
        return 0;
    }
	

# OUTPUT:
 

# QUESTION 12:	
#### Write a program that gets array elements as input from a user and then asks the user to input any value to search from the array. After that, if the value entered by the user is present in the array, it should display the index where that value is present. If the value is NOT present in the array, then it should print a message saying that the given value is not present in the array. 

## CODE:

    #include <iostream>
    using namespace std;
    
    int main() {
        int n;
        cout << "Enter the size of the array: ";
        cin >> n;
    
        int arr[n];
        cout << "Enter " << n << " elements:\n";
        for (int i = 0; i < n; i++) {
            cin >> arr[i];
        }
    
        int key;
        cout << "Enter the value to search: ";
        cin >> key;
    
        bool found = false;
        for (int i = 0; i < n; i++) {
            if (arr[i] == key) {
                cout << "Value " << key << " is found at index: " << i << endl;
                found = true;
                break;  
            }
        }
    
        if (!found) {
            cout << "Value " << key << " is not present in the array.\n";
        }
    
        return 0;
    }
    
# OUTPUT:
 

