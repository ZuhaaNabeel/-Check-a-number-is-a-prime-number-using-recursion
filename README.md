# -Check-a-number-is-a-prime-number-using-recursion
Create a C++ program to check a number is a prime number or not using recursion

/* Create a C++ program to check a number is a prime number or not using recursion*/
 
 #include<iostream>
 using namespace std;
 bool prime(int n,int l)
 {

 	if(n<2)
 	{
 		return true;
	}

	   
		if(n%l==0)
		{
			return false;	
		}

	 prime(n,l-1);

 }
 int main()
 {
 	cout<<"Enter a number you want to find whether its prime or not"<<endl;
 	int k;
 	cin>>k;
 	int z=k;
 	cout<<prime(k,z-1)<<endl;
 
 }
