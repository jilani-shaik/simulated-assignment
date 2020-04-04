# simulated-assignment
10 students
#include<stdio.h>
int main()
{
      int a[10],i,h,k;
      char b[10],k1;
     for(i=0;i<10;i++)
      b[i]=(char)(97+i);
      printf("Enter Gifts taken by 10 students\n");
      for(i=0;i<10;i++)
{            
        printf("for %c student : \t",b[i]);
    
      scanf("%d",&a[i]);
}
h=0;
for(;h==0;)
{
   h=1;
  for(i=0;i<9;i++)
{
 if(a[i]<a[i+1])
 {
  k=a[i];
  a[i]=a[i+1];
  a[i+1]=k;
  k1=b[i];
  b[i]=b[i+1];
  b[i+1]=k1;
  h=0;}
  }
  }
printf("The order is \n");
printf("-------------------------------------------------\n");
printf("Students \t   no of gifts\n");
printf("-------------------------------------------------\n");
for(i=0;i<10;i++)
{
 if(a[i]>0)
printf(" %c \t\t\t %d\n", b[i],a[i]);
 else
 continue;
}
}
