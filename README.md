# suite-de-Fibonacci-
avec fct de récursivité

#include <stdio.h>

int suite_fibonacci(int N){

    if(N==0){
        return 0;
    }
    
    else if(N==1){
        return 1;
    }
    
    else{
        return suite_fibonacci(N-1)+suite_fibonacci(N-2);
    }
    
}

int main() {

int n,i;

printf("veuiller entrer un nbre ou un degre que voulez vous ");
scanf("%d",&n);
printf("la suite de fibonacci de votre nbre %d ou de votre degre est : \n ",n);

for(i=0;i<n;i++){

printf(" %d  \n ",suite_fibonacci(i));

}

    return 0;
}
