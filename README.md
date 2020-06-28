#include <stdio.h>
int main(void)
{
int a[5]={1,2,3,4,5},n,b,found;
printf("enter the number to be searched:");
scanf("%d",&n);
printf("enter the number to be updated:");
scanf("%d",&b);
for(int i=0;i<5;i++)
{
  if(n==a[i])
  {
    a[i]=b;
    found=1;
    break;
  }
}
if(found==1)
{
  printf("the updated array is: ");
  for(int i=0;i<5;i++)
  {
    printf("%d ",a[i]);
  }
}
else
printf("the element is not found");

  return 0;
}
