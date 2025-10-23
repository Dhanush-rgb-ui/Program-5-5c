# Module-5 Day-3 SEB
## AIM:
To write a C program to read matrix [3x3] that prints the sum of major(main) and minor(off) diagonal element:

## For example:
<img width="351" height="292" alt="image" src="https://github.com/user-attachments/assets/04063ee2-0890-4f0e-b5cb-315cf51c427a" />


## Program:
```c
#include <stdio.h>
int main()
{
    int n=3;
    int a[n][n];
    int i,j;
    int sum1=0,sum2=0;
    for(i=0;i<n;i++){
        for(j=0;j<n;j++){
            scanf("%d ",&a[i][j]);
        }
    }
    for(i=0;i<n;i++){
        for(j=0;j<n;j++){
            printf("%d ",a[i][j]);
        }
        printf("\n");
    }
    printf("\n");
    printf("Major Diagonal Elements : ");
    for(i=0;i<n;i++){
        for(j=0;j<n;j++){
            if(i==j){
                printf("%d ",a[i][j]);
                sum1+=a[i][j];
            }
        }
    }
    printf("\n");
    printf("\nMinor Diagonal Elements : ");
    for(i=0;i<n;i++){
        for(j=0;j<n;j++){
            if(j==n-1-i){
                printf("%d ",a[i][j]);
                sum2+=a[i][j];
            }
        }
    }
    printf("\n");
    printf("\nSum of Major Diagonal Elements : %d",sum1);
    printf("\n");
    printf("\nSum of Minor Diagonal Elements : %d",sum2);
    return 0;
}
```
## Result:
<img width="727" height="550" alt="image" src="https://github.com/user-attachments/assets/f6347b6e-b123-4110-b7c1-0920a1dad26e" />
