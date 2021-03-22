```
#include<stdio.h>

void tamil();
void english();
void malayalam();
void hindi();
void time();
void payment();
void board();
int square[17] = { 0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16 };
int main()
{
	int i, choice;
    int mark;
	int userchoice;
	
	while(1)
	{
		printf("\n***ONLINE TICKET BOOKING***");
	    printf("\n\nMOVIE DETAILS:");
	    printf("\n\n1)TAMIL\n2)ENGLISH\n3)MALAYALAM\n4)HINDI\n");
	    printf("\n\nENTER THE CHOICE:");
	    scanf("%d",&userchoice);
	    
	    switch(userchoice)
	    {
	    	case 1:tamil();
	    	   break;
	        case 2:english();
	    	   break;
		    case 3:malayalam();
	    	   break;
		    case 4:hindi();
	    	   break;			
	        default :printf("wrong choice!!");  
	        
		}
		
        do
        {
        	board();
            mark=0;

            printf("\n\n ENTER YOUR SEAT CHOICE:");
            scanf("%d", &choice);
           
            if (choice == 1 )
            
                square[1] = mark;
               
            
            else if (choice == 2 )
                square[2] = mark;
            
            else if (choice == 3 )
                square[3] = mark;
            
            else if (choice == 4 )
                square[4] = mark;
            
            else if (choice == 5 )
                square[5] = mark;
            
            else if (choice == 6 )
                square[6] = mark;
            
            else if (choice == 7 )
                square[7] = mark;
            
            else if (choice == 8 )
                square[8] = mark;
            
            else if (choice == 9 )
                square[9] = mark;
          
	     	else if (choice == 10 )
                square[10] = mark;
			
		    else if (choice == 11 )
                square[11] = mark;
			
	    	else if (choice == 12 )
                square[12] = mark;
			
    		else if (choice == 13 )
                square[13] = mark;
			
	    	else if (choice == 14 )
                square[14] = mark;
			
		    else if (choice == 15 )
                square[15] = mark;
			
		    else if (choice == 16 )
                square[16] = mark;						    
            
            else
            {
            	printf("Invalid move ");
                getch();
			}
        
        }while (i ==   0);
        board();
        payment();
        }
}
	
		
void tamil()
{
	int moviechoice;
	printf("\n\n1)SINDHUBAADH - Rs.100\n2)KADARAM KONDAN - Rs.100\n3)THE LION KING - Rs.100\n");
	printf("\n\nENTER THE CHOICE:");
	scanf("%d",&moviechoice);
	time();
}

void english()
{
	int moviechoice;
	printf("\n\n1)ANGRY BIRD - Rs.100 2\n2)KINGS - Rs.100\n3)BLACE - Rs.100\n");
	printf("\n\nENTER THE CHOICE:");
	scanf("%d",&moviechoice);
	time();
}

void malayalam()
{
	int moviechoice;
	printf("\n\n1)PREMAM - Rs.100\n2)SACHIN - Rs.100\n3)MAARCONI MATHAAI - Rs.100\n");
	printf("\n\nENTER THE CHOICE:");
	scanf("%d",&moviechoice);
	time();
}

void hindi()
{
	int moviechoice;
	printf("\n\n1)MERI BHAGYA LAKSHMI - Rs.100\n2)FORTY PLUS - Rs.100\n3)HYDERABAD NAWABS 2 - Rs.100\n");
	printf("\n\nENTER THE CHOICE:");
	scanf("%d",&moviechoice);
	time();
}
	
void time()
{
	int timechoice;
	printf("\n\n1)MORNING : 9.00AM-12.00PM\n");
	printf("2)AFTERNOON : 1.00PM-4.00PM\n");
	printf("3)EVENING : 6.00PM-9.00PM\n");
	printf("4)NIGHT : 10.00PM-1.00AM\n");
	printf("\n\nENTER TIME CHOICE:");
	scanf("%d",&timechoice);
}

void board()
{
    printf("\n\n     |     |     |     |\n");
    printf("  %d  |  %d  |  %d  |  %d  |\n", square[1], square[2], square[3], square[4]);
    printf("_____|_____|_____|_____|\n");

   
    printf("     |     |     |     |\n");
    printf("  %d  |  %d  |  %d  |  %d  |\n", square[5], square[6], square[7], square[8]);
    printf("_____|_____|_____|_____|\n");
   
   
    printf("     |     |     |     |\n");
    printf("  %d  |  %d | %d  | %d  |\n", square[9], square[10], square[11], square[12]);
    printf("_____|_____|_____|_____|\n");

   
    printf("     |     |     |     |\n");
    printf("  %d |  %d | %d  | %d  |\n", square[13], square[14], square[15], square[16]);
    printf("_____|_____|_____|_____|\n");
}

void payment()
{
	char name[20];
	int cardno;
	int cvv;
	int expiry;
	int amount;
	
	printf("\n\nNAME:\n");
	scanf("%s",name);
	printf("\n\nEnter 16 digit number from debit card\n");
	printf("CARD NUMBER:\n");
	scanf("%d",&cardno);
	printf("\n\nEnter MM/YY from debit card\n");
	printf("EXPIRY DATE:\n");
	scanf("%d",&expiry);
	printf("\n\nEnter 3 digit CVV number from debit card\n");
	printf("CVV:\n");
	scanf("%d",&cvv);
	printf("\n\nAMOUNT:");
	scanf("%d",&amount);
	printf("\n\nPAYMENT SUCCESSFULL\n\n");
	printf("***********************************************************\n");
	printf("               %s, TICKED BOOKED SUCCESSFULLY              \n", name);
	printf("***********************************************************\n\n");
}
```
