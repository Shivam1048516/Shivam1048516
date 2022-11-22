/******************************************************************************

                              Online C++ Compiler.
               Code, Compile, Run and Debug C++ program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <iostream>

using namespace std;

int main()
{
  int arr[10], tot=10, i, elem, j, found=0;
  cout<<"enter 7 array elements:";
  for(i=0; i<tot; i++)
  cin>>arr[i];
  cout<<"\nenter element to delete:";
  cin>>elem;
  for(i=0; i<tot; i++)
  {
      if(arr[i]==elem)
      {
          for(j=i; j<(tot-1); j++)
          arr[j]= arr[j+1];
          found++;
          i--;
          tot--;
          
      }
  }
 if(found==0)
 cout<<"\nelement doesnot found in the array!";
 else
 cout<<"\nelement deleted successfully!";
 cout<<endl;
    return 0;
}
