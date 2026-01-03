# C-program-to-fill-employee-details
Employee salary  details 
#include<stdio.h>
struct employee{
 char name[100];
 int salary,age;
};
int main(){
 int n;
 printf("enter the number of employees:");
 scanf("%d",&n);
 struct employee e[n];
 for(int i=0;i<n;i++){
 printf("\nEnter the employee name:");
 scanf("%s", e[i].name);
 printf("Enter the salary:");
 scanf("%d",&e[i].salary);
 printf("Enter the age:");
 scanf("%d",&e[i].age);
 }
 printf("\n information \n");
 for(int i=0;i<n;i++){
 printf("\nName:%s\n",e[i].name);
 printf("Salary:%d\n",e[i].salary);
 printf("Age:%d\n",e[i].age);
 }
 return 0;
}