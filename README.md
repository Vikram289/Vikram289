#include <stdio.h>

int main()
{
    float x,y;
    char ch;
    printf("Enter Intital Ammount\n");
    scanf("%f",&x);
    printf("Enter\nc for credit\nd for debit\nb for balance\n");
    scanf("\n%c",&ch);
    switch(ch)
    {
       
 case 'c':
        printf("Enter Credit Ammount\n");
        scanf("%f",&y);
        x=x+y;
        printf("New Ammount=%f",x);
        break; 
        
        case 'd':
        printf("Enter Debit Ammount\n");
        scanf("%f",&y);
        if(x>y)
        {
            x=x-y;
            printf("New Ammount=%f",x);
        }
        else {
            printf("Insufficient Balance");
        }
        break;
        
        
case 'b':
        printf("Ammount in your account=%f",x);
        break;
        
        default:
        printf("Invalid option");
        
    }
    return 0;
}
