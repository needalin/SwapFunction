SwapFunction (C++)
============
.cpp File
------
'''
    // ConsoleApplication30.cpp : Defines the entry point for the console application.

    #include "swapfunction.h"
    #include <iostream>
    #include <algorithm> // for swap
    using namespace std;
    
    void swap (int secondarray[], int length) // defines the parameter and length 
 	{
  	for (int n=0; n<length; n++)
  	cout << secondarray[n] << " ";
  	cout << "\n";
	}

	int main()
	{
	array functionswap;
	functionswap.getarray();
	functionswap.printarray();
	
	 return 0;
	}
	
'''
HEADER FILE:
------

'''
    #include <iostream>
    #include "algorithm" // for swap
    using namespace std;

    class array

    	{
	public:
	void getarray(); // obtain varibles 
	void printarray(); // swap and output variables
	
	private:
	int x;
	int y;
	int z;
	int t;
	int firstarray;
	int secondarray;
   	};

    	void array::getarray()
    	{
	cout << "please enter four numbers. The first and last numbers will be swapped:\n\n";
	cout << "Enter number one \n";
	cin >> x;
	cout << "Enter number two \n";
	cin >> y;
	cout << "Enter number thee \n";
	cin >> z;
	cout << "Enter number four \n";
	cin >> t;
	cout << "\nHere are the original set of values you entered: \n\n";
	
	int firstarray[4] = {x, y, z, t};
	
	cout << x << y << z << t; //summary of values put in
	}
	
	void array::printarray()
	
	{
	
	swap(x, t); // swap placement of only variables x, t
 
	cout << "\n\nHere are your numbers, with the first and last numbers swapped \n\n";
	
	int firstarray[4] = {x, y, z, t};//this is the original order
	
	cout << x << y << z << t;//this is the swapped output
	cout << "\n\n";
	
	}
	'''
