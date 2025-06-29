#include <iostream>
using namespace std;


int main()
{
    int count=0,n;
    
    cout<<"enter number of elements of array"<<endl;
    
    cin>>n;
    
     int array [n]  ;
     
     for(int i=0;i<n;i++)
     {
         cout<<"enter the element ";
         
         cin>>array[i];
     }
     
     for(int i=0;i<n;i++)
     {
         for(int j=i+1;j<n;j++)
         {
             if(array[i]>array[j])
             {
                  count++;
             }
         }
     }
     
     if(count>0)
     {
         cout<<"the array is unsorted";
     }
     
     else
     {
         cout<<"the array is  sorted";
     }

    return 0;
}
