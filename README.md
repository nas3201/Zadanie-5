#include "stdafx.h"
#include "iostream"
#include "math.h"
 
 //yi+1 = 0.5(yi + 3x/(2pow(yi,2) + x /уi)).
int main()
{
    float x,y,a;
    printf("Vvedite x:\n");
    scanf("%f",&x);
    y = x;
    a = 0;
    while(fabs(y-a)>pow(10, -5))
    {            
        a=y;
        y=0.5*(a+(3*x)/(2*pow(a, 2)+x/a)); 
    }
 
    printf("%f",y);
    return 0;
}
