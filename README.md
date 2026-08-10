#include<stdio.h>

int main()
{
    void primecheck();
    primecheck();
    return 0;
}

void primecheck()
{
    int a,i,flag=0;
    scanf("%d",&a);
    if(a<=1) flag=1;
    else{
        for(i=2;i<=a/2;++i)
        {
            if(a%i==0)
            {
                flag=1;
                break;
            }
        }
    }
    if(flag==1)printf("NOT prome");
    else printf("PRIME");

}
