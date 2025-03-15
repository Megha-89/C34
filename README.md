# C34
Insertion of array 
#include <stdio.h>
int main()
{
int n,i,value,pos;
printf("enter the number of numbers:");
scanf("%d",&n);
int arr[n+1];
printf ("enter %d elements:\n",n);
for(i=0;i<n;i++){
scanf ("%d",&arr[i]);
}
printf ("enter the element to insert :");
scanf("%d",&value);
printf ("enter the position ");
scanf("%d",&pos);
for(i=n;i>=pos;i--){
arr[i]=arr[i-1];
}
arr[pos-1]=value;
n++;
printf ("after insertion: \n");
for(i=0;i<n;i++)
{
printf("%d ",arr[i]);
}
printf ("\n");
return 0 ;
}
