
# Question 01:
#### Write a C++ program that maintain record of students. Student contains following 
details: 
a) ID 
b) Name 
c) Department 
d) Email 
e) Phone number 
 
#### Create a structure names Student. Ask the user to enter record for 5 students and 
#### store those details in variables of Student type. Finally, print those records on screen.


## Code:

    #include <iostream>
    using namespace std;
         struct student{
         	int id;
         	string name;
         	string department;
         	string email;
         	string phoneNumber;
    	 }
    	int main(){
    	   student s[5];
    	   cout<<"Enter record of 5 students: \n\n";
    	   for(int i=0; i<5; i++){
    	   	cout<<"student"<<i+1<<":\n";
    	   	cout<<"Enter ID: ";
    	   	cin>>s[i].id;
    	   	cin.ignore();
    	   	cout<<"Enter Name: ";
    	   	getline(cin,s[i].name);
    	   	cout<<"Enter Department: ";
    	   	getline(cin, s[i].department);
    	   	cout<<"Enter Email: ";
    	   	getline(cin,s[i].email);
    	   	cout<<"Enter Phone number: ";
    	   	cin>>s[i].phoneNumber;
    	   	cin.ignore();
    	   	cout<<endl;
    	   }
    	     cout << "----- Student Records -----\n\n";
        for (int i = 0; i < 5; i++) {
            cout << "Student " << i + 1 << ":\n";
            cout << "ID: " << s[i].id << endl;
            cout << "Name: " << s[i].name << endl;
            cout << "Department: " << s[i].department << endl;
            cout << "Email: " << s[i].email << endl;
            cout << "Phone: " << s[i].phoneNumber << endl;
            cout << "------------------------------\n";
        }		
    	 return 0 ;}	


# OUTPUT:
 

<img width="654" height="1086" alt="ChatGPT Image Jun 10, 2026, 03_38_04 PM" src="https://github.com/user-attachments/assets/bd4c5625-faa0-4682-b46c-237426371905" />









<img width="673" height="1086" alt="ChatGPT Image Jun 10, 2026, 03_41_18 PM" src="https://github.com/user-attachments/assets/2d0093b4-7b7e-486e-b437-510c27e2e54b" />



















# Question 02: Write a C++ program to do:
##### a) Create a structure/record to store products; each product has a name, a model number and a price. 
##### b) Choose appropriate types for these fields/attributes.
##### c) Your program should contain a loop which allows entry via the keyboard of up to 10 products, and stores them in an array 
##### d) Finally, the program should include a function to display all the products details after the entry loop has finished.

## CODE:
    
    #include <iostream>
    using namespace std;
    struct Product {
        string name;
        int modelNumber;
        float price;
    };
    
    void displayProducts(Product p[], int count) {
        cout << "\n----- Product Details -----\n\n";
        for (int i = 0; i < count; i++) {
            cout << "Product " << i + 1 << ":\n";
            cout << "Name: " << p[i].name << endl;
            cout << "Model Number: " << p[i].modelNumber << endl;
            cout << "Price: $" << p[i].price << endl;
            cout << "-----------------------------\n";
        }
    }
    
    int main() {
    
        Product products[10];   
        int count = 0;         
        cout << "Enter product details (up to 10 products) \n";
        cout << "Press 0 as model number to stop entry.\n\n";
    
        for (int i = 0; i < 10; i++) {
            cout << "Product " << i + 1 << ":\n";
    
            cout << "Enter Model Number (0 to stop): ";
            cin >> products[i].modelNumber;
    
            if (products[i].modelNumber == 0) {
                break; 
            }
    
            cin.ignore(); 
            cout << "Enter Name: ";
            getline(cin, products[i].name);
    
            cout << "Enter Price: ";
            cin >> products[i].price;
    
            cout << endl;
    
            count++; 
        }
    
       
        displayProducts(products, count);
    
        return 0;
    }

 
# OUTPUT:

<img width="650" height="1142" alt="image" src="https://github.com/user-attachments/assets/2b6d7c24-b205-47dc-8a47-0d78ed577dcb" />

 



# Question 03
#### Write a C++ program that compute Net Salary of Employee. Program should contain two user defined functions empSalary( ) and display( ).
 ##### a) Create a structure of Employee that contains following data members:
		 i. EmployeeNumber, Name, BasicSalary, HouseAllowance, MedicalAllowance, Tax, GrossPay and NetSalary            
 ##### b) EmployeeNumber, Name, and BasicSalary should be taken input from the user
 ##### c) The function empSalary( ) should compute the Employee salary with given criteria
 i. HouseAllowence = 10% of BasicSalary
 ii. Medical Allowence = 5% of Basic Salary 
iii. Tax = 4 % of Basic Salary 
iv. GrossSalary = Basic+HouseAllowence+MedicalAllowence
 v. NetSalary = GrossSalary – Tax
##### d) The function display() should display the details of Employee, like shown below:

## CODE:

    #include <iostream>
    using namespace std;
    struct Employee{
    	string EmployeeNumber;
    	string Name;
    	float BasicSalary;
    	float HouseAllowance;
    	float MedicalAllowance;
    	float Tax;
    	float GrossPay;
    	float NetSalary;
    };
    	void empSalary(Employee &emp){
    		emp.HouseAllowance = (emp.BasicSalary) * (10.0 / 100);
    		emp.MedicalAllowance = (emp.BasicSalary) * (5.0 / 100);
    		emp.Tax = (emp.BasicSalary) * (4.0 / 100);
    		emp.GrossPay = (emp.BasicSalary) + (emp.HouseAllowance) + (emp.MedicalAllowance);
    		emp.NetSalary = (emp.GrossPay) - (emp.Tax);
    	}
    
    	void display(Employee &emp){
    		cout<<"\n\n****************************************\n\n";
    		cout<<"       EMPLOYEERS SALARY DETAILS\n\n";
    		cout<<"****************************************\n";
    		cout<<"Employee Number: "<<emp.EmployeeNumber<<endl;
    		cout<<"Employee Name: "<<emp.Name<<endl;
    		cout<<"Employee Basic Salary: "<<emp.BasicSalary<<endl;
    		cout<<"Employee House Allowance: "<<emp.HouseAllowance<<endl;
    		cout<<"Employee Medical Allowance: "<<emp.MedicalAllowance<<endl;
    		cout<<"Employee Gross Salary: "<<emp.GrossPay<<endl;
    		cout<<"Employee Tax Deduction: "<<emp.Tax<<endl;
            cout<<"Employee Net Salary: "<<emp.NetSalary<<endl;
    	}
    		int main(){
    			Employee emp;
    			cout<<"Enter Employee Number: ";
    			cin>>emp.EmployeeNumber;
    			cin.ignore();
    			cout<<"Enter Employee Name: ";
    			getline(cin,emp.Name);
    			cout<<"Enter Employee Basic Salary: ";
    			cin>>emp.BasicSalary;
    			
    			empSalary(emp);
    			
    			display(emp);
    	
        return 0;
    }

    
# OUTPUT:

<img width="786" height="781" alt="image" src="https://github.com/user-attachments/assets/56f2bb48-aa74-4b31-ae97-b08e7d1c8448" />


 
 
# QUESTION 04:
#### Consider the following code:

    #include <string>  
    #include <iostream>  
    using namespace std; 
    struct Student {  
    string name;  
    int id; 
    int mark[3]; 
    }; 
    void inputStudent(Student* ptr); //function prototype for getting input 
    // some other function for printing the details 
    //*********************** Main Function ************************//  
    int main () { 
    Student stu; // declaring an Student object  
    Student* stuPtr = &stu; // defining a pointer for the object 
    inputStudent(&stu); // calling function to get input into the object 
    // calling the other function to print the details of the object 
    return 0; 
    } // end main 
     
   #### In above given code there is a prototype, and a call to a function to input the values into a Student instance. Note that the parameter to this function is the address of a structure instance. 
     
    a) Write the definition for this function at the bottom of the file. 
    b) Then, write a function that takes a pointer to an instance of the Student structure and displays the contents 
    
    
  ## CODE:
      #include <string>  
      #include <iostream>  
      	using namespace std; 
      	struct Student {  
      	string name;  
      	int id; 
      	int mark[3]; 
      	}; 
      	void inputStudent(Student* ptr);
      	
      	void display(Student* ptr);
      	
      	  
      	int main () { 
      	Student stu;  
      	Student* stuPtr = &stu; 
      
      	cout<<"***Input student Information***\n";
      	inputStudent(&stu);
      	cout<<"***Details of the Students***\n";
      	display(&stu);
      		
      	return 0; 
      }
      
      	void inputStudent(Student* ptr){
      	cout<<"Enter the Name of the Student: ";
      	getline(cin,(*ptr).name);
      	cout<<"Enter Student ID: ";
      	cin>>(*ptr).id;
      	cin.ignore();
      	for(int i=0; i<3; i++){
      	cout<<"Enter Marks "<<i+1<<": ";
      	cin>>(*ptr).mark[i];
      	}
      }
      	
      		void display(Student* ptr){
      		cout<<"Name: "<<(*ptr).name<<endl;
      		cout<<"ID: "<<(*ptr).id<<endl;
      		for(int i=0; i<3; i++){
      		cout<<"Marks: "<<(*ptr).mark[i]<<endl;
      		}
      	}

      
  # OUTPUT:
 
<img width="647" height="532" alt="image" src="https://github.com/user-attachments/assets/22681ea1-2c67-4c58-99d1-609ec78db8c6" />



 
# Question 05: Making and Using Dynamically Allocated Arrays. 
#### Let us say that you want to choose how many marks to enter for the student and have the array change size accordingly. This gives you the opportunity to work with dynamic pointers. 
#### You will have to make the following changes to the code previously given: 
 
a) Change mark within the Student struct to an integer pointer. 
b) Ask the user from main how many marks he/she would like to enter 
c) Change both the functions to have an additional parameter which is the number of marks. 
d) For the inputStudent function, dynamically allocate the marks according to the number required.


## CODE:

    #include <string>  
    #include <iostream>  
    	using namespace std; 
    	struct Student {  
    	string name;  
    	int id; 
    	int* mark; 
    	}; 
    	void inputStudent(Student* ptr, int numMarks);
    	
    	void display(Student* ptr, int numMarks);
    	
    	  
    	int main () { 
    	int numMarks;
        cout<<"Enter How Many Marks You want to enter: ";
        cin>>numMarks;
        cin.ignore();
    	Student s;
    
    	cout<<"***Input student Information***\n";
    	inputStudent(&s  , numMarks);
    	cout<<"***Details of the Students***\n";
    	display(&s , numMarks);
    		
    	return 0; 
    }
    
    	void inputStudent(Student* ptr, int numMarks){
    	cout<<"Enter the Name of the Student: ";
    	getline(cin,(*ptr).name);
    	cout<<"Enter Student ID: ";
    	cin>>(*ptr).id;
    	cin.ignore();
    	(*ptr).mark = new int[numMarks];
    	
    	for(int i=0; i<numMarks; i++){
    	cout<<"Enter Marks "<<i+1<<": ";
    	cin>>(*ptr).mark[i];
    	}
    }
    	
    		void display(Student* ptr , int numMarks){
    		cout<<"Name: "<<(*ptr).name<<endl;
    		cout<<"ID: "<<(*ptr).id<<endl;
    		for(int i=0; i<numMarks; i++){
    		cout<<"Marks: "<<(*ptr).mark[i]<<endl;
    		}
    	}
    
# OUTPUT:

 <img width="580" height="611" alt="image" src="https://github.com/user-attachments/assets/c02a3c68-a330-48f4-bb80-7bea30ced210" />




