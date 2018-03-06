# Lab-4
Need this done before 1pm
1.	Write a program. Use for loop to output integer number from 1 to 10.  

2.	Write a program. Use for loop to input three integers and calculate the sum of three integers (sum = sum +num ;).  Output your result.

3.	Use for loop to input 4 numbers from keyboard. If the input number is positive, print “positive number” (num >=0 ;), otherwise print “negative number”. 

4.	Use while loop to solve problem 1.

5.	Write a program to calculate the sum of following series where n is input by user (for (i=1; i<=n; i++) sum = sum+1.0/i ;).
1 + 1/2 + 1/3 + 1/4 + 1/5 +…………1/n

6.
	Evaluating Equations with One Unknown 
Loops can be constructed to give you a way to determine and display the values of a single unknown in an equation for a set of values over any specified interval. For example, suppose you want to know the values of y in the following equation for x between 2 and 6:    y = 10x2 + 3x – 2
   Write a program for this example. Assuming x has been declared as an integer variable, use for loop to calculate the y value for each x between 2 and 6. Output your results. 
              y = 10 * pow(x,2.0) + 3 * x – 2;    //code for calculating y value for each x
cout << setw(4) << x << setw(11) << y << endl; //code for output each x and y

==============================================
Code Examples
Example for loop
#include <iostream>
using namespace std;

int main(){
  int count;

  for (count = 1; count <= 20; count = count + 1)
    cout << count << " ";

  return 0;
}

Example for loop
#include <iostream>
using namespace std;

int main()
{
  const int MAXNUMS = 4;
  int count;
  int num;

  cout << "\nThis program will ask you to enter "
       << MAXNUMS << " numbers.\n";

  for(count=1;count <= MAXNUMS;count++)
  {
    cout << "\nEnter a number: ";
    cin  >> num;
    cout << "The number entered is " << num;
  }
  cout << endl;

  return 0;
}

Example do while loop
do
{
  cout << "\nEnter an identification number: ";
  cin >> idNum;
  if (idNum < 100 || idNum > 1999)
  {
cout << "\n An invalid number was just entered"
     << "\nPlease check the ID number and reenter";
         }
else
	   break; // break if a valid ID number was entered
} while(1); // this expression is always true
