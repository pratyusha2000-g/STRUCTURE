# STRUCTURE
DISPLAYING DETAILS OF 20 EMPLOYEE USING STRUCTURE
#include<stdio.h>
#include<string.h>
void display(struct employee details[20]);
struct employee
{
    int empno,salary;
    char empname[100],dep_name[100];
};

int main()
{
   int i;
   struct employee details[20];
   printf("Enter the details of 20 employee \n");
   printf("Employee number Employee Name Department Name Salary \n");
   for(i=0;i<20;i++)
   {
      printf("Enter employee number \n");
      scanf("%d",&details[i].empno);
      
      printf("Enter employee name \n");
      gets(details[i].empname);
      
      printf("Enter department name \n");
      gets(details[i].dep_name);
      
      printf("Enter salary of the employee \n");
      scanf("%d",&details[i].salary);
     }  
       display(details);
      return 0;
   }

void display(struct employee details[20])
{
   int i;
   printf("DISPLAYING EMPLOYEE NUMBER , EMPLOYEE NAME , DEPARTMENT NAME, SALARY \N");

  for(i=0;i<20;i++)
   {
     
    printf("%d , %s , %s , %d \n",details[i].empno,details[i].empname,details[i].dep_name,details[i].salary);
     }  
   
}
