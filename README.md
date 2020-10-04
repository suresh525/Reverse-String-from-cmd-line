# Reverse-String-from-cmd-line
#include<stdio.h>
#include<string.h>
int main(int argc,char *argv[])
{
        if(argc!=2){
                printf("use:./list string\n");
                return 0;
        }
        int i,j,k;
        char a[50],temp;
        strcpy(a,argv[1]);

        for(i=0,j=strlen(a)-1;i<j;i++,j--)
        {
                if(a[i]!=a[j])
                {
                temp=a[i];
                a[i]=a[j];
                a[j]=temp;
                }

        }
        printf("Output:%s",a);

}
