# include<stdio.h>
int main(void)
{
    char c;
    int m=0, n=0, j=0, k=0;

    while((c=getchar())!='\n')
    {

        if(c==' ')
            ++n;
        else if(c>='0'&&c<='9')
            ++j;
        else if((c>='a'&&c<='z')||(c>='A'&&c<='Z'))
            ++k;
        else ++m;
    }

    printf("number %d\n english %d\n space %d\n else %d\n",j,k,n,m  );
    return 0;
