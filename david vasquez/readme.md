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

### _CÛdigo en c++_

```
#include<iostream>
#include<cmath>
#include<stdio.h>
using namespace std;
int lis[101];
int dic[100001];
float precio[100001];
float matriz[101][100001];
int main()
{
    const unsigned int infinito=pow(2,31);
    int M,N;
    scanf("%d %d",&M,&N);
    int j;
    while(M || N){
        for(int i=0;i<M;i++){
            cin>>lis[i];
        }
        for(int i{0};i<N;i++){
            cin>>dic[i];
            cin>>precio[i];
        }


        for(int j=0;j<=N;j++){
            matriz[M][j]=0;
        }

        for(int i=M-1;i>-1;i--){
            j=N-1;
            matriz[i][N]=infinito;
            while(i<=j && j>-1){
                matriz[i][j]=infinito;
                if(lis[i]==dic[j]){
                    matriz[i][j]=min(matriz[i+1][j+1]+precio[j],matriz[i][j+1]);
                }

                else{
                    matriz[i][j]=min(matriz[i][j+1],matriz[i][j]);
                }
                j--;
            }


        }
        if(matriz[0][0]!=infinito){
            printf("%.2lf\n", matriz[0][0]);

        }
        else{
            printf("Impossible\n");

        }
        scanf("%d %d",&M,&N);
    }
    return 0;
}

```
