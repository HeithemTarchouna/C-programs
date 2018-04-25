# Sorting-Algorithm
C program
#include <stdio.h>

int main()
{
    int tab[5];
    int i=0;
    int temp;
    int j=0;
    for(i=0;i<5;i++){
    printf("Element[%d] = ",i+1);
        scanf("%d",&tab[i]);
    }
    for(i=0;i<4;i++){
        for(j=i+1;j<5;j++){
        if (tab[i]<=tab[j]){
            temp=tab[i];
            tab[i]=tab[j];
            tab[j]=temp;
        }
        }
    }
    return 0;
}
