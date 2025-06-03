#include <stdio.h>

int main()
{   
    int sub1;
    int sub2;
    int sub3;
    float avg;
    float total;
    
    printf("enter the subject1 marks\n");
    scanf("%d",&sub1);
    printf("enter the subject2 marks\n");
    scanf("%d",&sub2);
    printf("enter the subject3 marks\n");
    scanf("%d",&sub3);
    
    total = sub1+sub2+sub3;
    avg = total/3;
   
    //scanf("%d,%d",&avg,&total);
    
    printf("subject1:%d\n ",sub1);
    printf("subject2:%d\n ",sub2);
    printf("subject3:%d\n ",sub3);
    printf("total:%.2f\n ",total);
    printf("avg:%.2f\n ",avg);
    
    
    if (sub1>=35 && sub2>=35 && sub3>=35){
        if ( avg>=70){
            printf("grade = FCD");
        
        }
        else if (avg>=60 && avg<70){
            printf("grade = FC");
        }
        else if (avg>=50 && avg<60){
            printf("grade = SC");
        }
    }
      
    else
    {
        printf("fail");
    }
    
    return 0;
}
