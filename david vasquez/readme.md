# Informacion

__David Alejandro Vasquez Carre—o__

_19 a—os_

Estudiante de ingenieria\
Nacido en 1999\
En Diciembre
### Actividaedes favoritas
- Videojuegos
- Dormir

### Plan de estudios
1) FCFI
2) ACSO
3) PRYE
4) CNYT
5) CVDS

![plan de estudios](https://www.escuelaing.edu.co/escuela/planesEstudio/img/sistemas/Malla-curricular-SISTEMAS.png)

### CÛdigo en c++

```
#include<iostream>
#include<limits.h>
#include<stdio.h>
using namespace std;
unsigned int lis[500000];
int n;
int ways(int i){
    unsigned int a;
    if(i==n-1){return 0;}
    if(i>0 && lis[i-1]>lis[i+1]){
        a=lis[i];
        lis[i]=lis[i+1];
        lis[i+1]=a;
        return 1+ways(i-1);
    }
    if(lis[i]>=lis[i+1]){
        a=lis[i];
        lis[i]=lis[i+1];
        lis[i+1]=a;
        return 1+ways(i+1);
    }
    return ways(i+1);
}
int main(){
    scanf("%d",&n);
    while(n){
        for(int i=0;i<n;i++){
            scanf("%d",&lis[i]);
        }
        printf("%d\n",ways(0));
        scanf("%d",&n);
    }
    return 0;
}

```
