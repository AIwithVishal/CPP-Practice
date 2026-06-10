
# Question 01 
#### Initialize an integer array of 5 elements. Then, print values of all elements along with their addresses using pointers.

## CODE:

    #include <iostream>
    using namespace std;
    int main(){
        
        int arr[5] = {3,5,8,9,12};
        int *ptr;
        cout<<"------Values in Array------\n";
        for(int i=0 ; i<5 ; i++){
        	cout<<"array [" << I << "] = " << arr[i] << endl;  	
    	}
    	cout<<"------Address in Array------\n";
    	 for(int i=0; i<5; i++){
        	cout<<"array ["<<i<<"] = "<< ptr + I <<endl;
    	}
      return 0 ;
    }
    
# Output:

<img width="647" height="476" alt="image" src="https://github.com/user-attachments/assets/9539eb77-5c2e-45d1-b6ca-2a42f0f10187" />


 
# Question 02: Pointer to Array 

#### Declare an array and a pointer to the array. Use the pointer to access and print elements of the array.

## CODE:

    #include <iostream>
    using namespace std;
    
    int main(){
        
        int arr[5] = {3,5,8,9,12};
        int *ptr = arr;
        cout<<"---Printing Elements in Array using Pointers---\n";
       		 for( int i=0 ; i<5 ; i++){
        	cout<<"                  "<<" arr[" << I <<"] = "<< *(ptr+i)<<endl;
    	}
        
      return 0 ;
    }
    
# OUTPUT:

<img width="898" height="406" alt="image" src="https://github.com/user-attachments/assets/ea11c3e9-e29a-4c6d-aa3f-f718debfb73d" />



 
# Question 03: Pointer Comparison
 #### Create two pointers pointing to different integer variables. Compare the values they point to and print whether they are equal or not.
 
## CODE:

    #include <iostream>
    using namespace std;
    
    int main(){
        int a = 6;
        int b = 9;
        int *ptr1 = &a;
        int *ptr2 = &b;
        cout << "Value pointed by ptr1 = " << *ptr1 << endl; 
        cout << "Value pointed by ptr2 = " << *ptr2 << endl;
      	cout<<endl;
        
        if(*ptr1==*ptr2){
        	cout<<"Both pointers point to EQUAL values. \n";
    	}else
    		cout<<"Both pointers point to DIFFERENT values. \n";
        
      return 0 ;
    }
    
# OUTPUT:

<img width="789" height="297" alt="image" src="https://github.com/user-attachments/assets/27f82458-766c-4f67-be8d-35dfbc31fc59" />



 
# Question 04: String Manipulation 
#### with Pointers Write a function that takes a string (array of characters) and reverses it using pointers.

## CODE:

    #include <iostream>
    using namespace std;
     void reversestring(char *str){
     	char *start = str;
     	char *end = str;
     	 while (*end != '\0') {     
            end++;
        }
        end--;
    	 
     	while(start<end){
     		char temp = *start;
     		*start = *end;
     		*end = temp;
     		
     		
     		*start++;
     		*end--;
    	 }
     	
     }
    int main(){
    	char str[] = "Excellent";
    	
    	cout << "String Before Reversing: " << str << endl;
    	 
    	reversestring(str);
    	
        cout << "String After Reversing: " << str << endl;
        
      return 0 ;
    }
    
# OUTPUT:

<img width="1037" height="270" alt="image" src="https://github.com/user-attachments/assets/29e17221-98da-4a64-a274-f96ae8bd65f0" />


 
# Question 05:
#### Write a program that should have a user-defined function names bubbleSort( ), which should have one parameter of pointer to an integer array. The function should sort the values of that array in ascending order (smaller to larger). Then, in the main( ) function, create an integer array initialized with some values within the code and print the array values along with a message saying that is the original/unsorted array values. After that, pass that array to the function bubbleSort( ) that should sort its values. Finally, print the array values along with a message saying that these are the sorted values.

## Code:

    #include <iostream>
    using namespace std;
        void bubblesort(int *ptr , int size){
        	
        	for(int i=0; i<size-1; i++){
        		
        	for(int j=0; j<size-i-1; j++){
        		
        		if(*(ptr + j)>*(ptr + j+ 1)){
        			
        			int temp = *(ptr +j );
        			*(ptr + j) = *(ptr + j+ 1);
        			*(ptr + j + 1) = temp;
        				
    				}
    			}
        	}
    	}
    	int main(){
    		 
    		 int arr[] = {5,67,3,24,9};
    		 int size = 5;
    		 
    		 cout<<"---Unsorted Array---\n\n";
    		 for(int i=0; i<size; i++){
    		 	cout<<arr[i]<<"  ";
    		 }
    		 cout<<endl;
    		 cout<<endl;
    		bubblesort(arr,size);
    		cout<<"---Sorted Array---\n\n";
    		 for(int i=0; i<size; i++){
    		 	cout<<arr[i]<<"  ";
    		 }
    		 cout<<endl;
    	 return 0 ;	
    	}
      
# OUTPUT:

<img width="957" height="546" alt="image" src="https://github.com/user-attachments/assets/377767a0-e229-412e-a7df-7b4560c6d871" />


 
 
# Question 06: 
#### Write a C++ program that creates an integer array of size 10. Then, get the array values as input from the user but save them in the array using a pointer. Then, print those values using the pointer Then, ask the user to search any value and perform a search operation using the pointer

## CODE:

    #include <iostream>
    using namespace std;
    	int main(){
    		 
    		 int arr[10];
    		 int *ptr = arr;
    		 
    		 cout<<"Enter 10 Integers: "<<endl;
    		 for(int i=0; i<10; i++){
    		 	cin>>*(ptr+i);
    		 }
    		 cout<<endl;
    		 cout<<"You Entered: "<<endl;
    		 for(int i=0; i<10; i++){
    		 	cout<<*(ptr+i)<<" ";
    		 }
    		 cout<<endl;
    		 
    		 int key;
    		 cout<<"\nenter the number you want to search: ";
    		 cin>>key;
    		 bool found = false;
    		 int index = -1;
    		 
    		 for(int i=0; i<10; i++){
    		 	if(*(ptr+i)==key){
    		 		found = true;
    		 		index = i;
    		 		break;
    			 }
    		 }
    		 if(found){
    		 	cout<<"Integer "<<key<<" found at index "<<index<<endl;
    		 }else
    		 	cout<<"Integer "<<key<<" dosen't found at any index "<<endl;	
    	 return 0 ;	
    	}
      
# OUTPUT:
    
<img width="744" height="397" alt="image" src="https://github.com/user-attachments/assets/dd3fe251-ca3e-4bb9-9f11-49e2c0481fa5" />


 
 
# Question 07: 
#### Create a function named swap( ) that should swap two integer values (means, exchanges the values between two variables; the value of first variable should be saved in the second one, and the value of the second variable should be saved in the first one, and so on) using pointers. The function parameters should be two pointers. Then, in the main( ) function, create (and initialize) two variables and print their values before calling the swap( ) function. After that, call the swap function. And finally, print those values after the function call to show that the values are swapped/exchanged.

## CODE:

    #include <iostream>
    using namespace std;
         
         	void swap(int *x , int *y){
    			int temp = *x;
    			*x = *y;
    			*y = temp;
    		}
    		
    	int main(){
    	   
    	   int a = 6;
    	   int b = 7;
    	   int *ptr1 = &a;
    	   int *ptr2 = &b;
    	   
    	   cout<<"Before Swapping: \n";
    	   cout<<"a"<< " = "<< *ptr1<<endl;
    	   cout<<"a"<< " = "<< *ptr2<<endl;
    	   
    	   swap(*ptr1 , *ptr2);
    	   
    	   cout<<"After Swapping: \n";
    	   cout<<"a"<< " = "<< *ptr1<<endl;
    	   cout<<"a"<< " = "<< *ptr2<<endl;
    		 
    		
    	 return 0 ;	
    	}
      
# OUTPUT:

<img width="644" height="331" alt="image" src="https://github.com/user-attachments/assets/16915150-2ea7-473d-a4ba-df65fef534e5" />




