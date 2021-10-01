<h1> Patterns:</h1>
This folder contains various type of patterns which is output of codes available here.
 #include<iostream>
using namespace std;
void right_triangle_pattern(int row)
{
    for (int i = 0; i < row; i++)
    {
        for (int j = 0; j <i; j++)
        {
            printf("*");
        }
        printf("\n");
    }
    
}
void equilateral_triangle_pattern(int rows)
{
    for(int i=1; i<= rows; i++) 
     {
           for(int j=i; j<rows; j++)
           {
                cout<<" ";
           }
           for(int j=1; j<=(2*i-1); j++)
           {
                cout<<"*";
           }

           cout<<"\n";
     } 
    
}
int main()
{
    int s,row;
    cout << "Enter number of rows in the triangle: ";
    cin >> row;
    printf("Type 1 for right tringle pattern\n Type 0 for equilateral triangle pattern: ");
    scanf("%d", &s);
    if (s==1)
    {
        right_triangle_pattern(row);
    }
    else if(s==0)
    {
        equilateral_triangle_pattern(row);
    }
    else
    {
        printf("Wrong Input");
    }
    return 0;
}
