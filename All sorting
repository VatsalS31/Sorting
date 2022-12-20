#include<stdio.h>
#define MAX 8
int input[MAX];
void bubblesort();
void insertionsort();
void selectionsort();
void countingsort();

void swap(int *x,int*y)
{
    int temp=*x;
    *x=*y;
    *y=temp;
}
int main()
{
    int ch;
     printf("BY VATSAL SHAH\n\n");
    do
    {
        printf("-------------WELCOME TO SEARCHING----------\n\n");
        printf("\n\n1.Bubble sort");
        printf("\n2.Insertion sort");
        printf("\n3.Selection sort");
        printf("\n4.Counting sort");
         
        printf("\nEnter the choice : ");
        scanf("%d",&ch);
        switch(ch)
        {
            case 1:
            bubblesort();

            break;
            case 2:
            insertionsort();
            break;
            case 3:
            selectionsort();
            break;
            case 4:
            countingsort();
            break;

        }
    }while(ch!=4);
}
void bubblesort()
{
    int i,j;
        printf("Enter the Elements to sort : \n");
        for(i=0;i<MAX;i++)
        {
        scanf("%d",&input[i]);
        
        }
        printf("\n");

    for(i=0;i<MAX-1;i++)
    {
        for(j=0;j<MAX-i-1;j++)
        {
            if(input[j]>input[j+1])
            {
                swap(&input[j],&input[j+1]);
            }
        }
    }
    for(i=0;i<MAX;i++)
    {
        printf("%d",input[i]);
        printf("\n");
    }iiiwi
}
void insertionsort()
{
     int i,j;
        printf("Enter the Elements to sort : \n");
        for(i=0;i<MAX;i++)
        {
        scanf("%d",&input[i]);
        
        }
        printf("\n");
        for(i=1;i<MAX;i++)
        {
            j=i-1;
            int x=input[i];
            while(j>-1 && input[j]>x)
            {
                input[j+1]=input[j];
                j--;
            }
            input[j+1]=x;
        }
        for(i=0;i<MAX;i++)
    {
        printf("%d",input[i]);
        printf("\n");
    }

}
void selectionsort()
{
    int i,j,k;
        printf("Enter the Elements to sort : \n");
        for(i=0;i<MAX;i++)
        {
        scanf("%d",&input[i]);
        
        }
        printf("\n");
        for(i=0;i<MAX-1;i++)
        {
            for(j=k=i;j<MAX;j++)
            {
                if(input[j]<input[k])
                {
                    k=j;
                }
            }
            swap(&input[i],&input[k]);
        }
        for(i=0;i<MAX;i++)
    {
        printf("%d",input[i]);
        printf("\n");
    }

}
void countingsort()
{
    int i,j;
    int c[MAX];
         
        printf("Enter the Elements to sort : \n");
        for(i=0;i<MAX;i++)
        {
        scanf("%d",&input[i]);
        
        }
        printf("\n");
        for(i=0;i<MAX+1;i++)
        {
            c[i]=0;             //intialising counter array with 0

        }
        for(i=0;i<MAX;i++)
        {
            c[input[i]]++;
        }
        i=0;j=0;
       
       while(i<MAX+1)
        {
            if(c[i]>0)
            {
                input[j++]=i;
                c[i]--;
            }
            else
            i++;


        }
         for(i=0;i<MAX;i++)
    {
        printf("%d",input[i]);
        printf("\n");
    }



}
