#include<stdio.h>
#include<string.h>
int main(){
    int matrixA[3][3];
    int matrixB[3][3];
    int matrixmulAB[3][3];
    for(int i=0;i<3;i++){
        for(int j=0;j<3;j++){
            printf("Enter %d and %d th element of matrix A: \n",i,j);
            scanf("%d",&matrixA[i][j]);
        }
    }
    for(int i=0;i<3;i++){
        for(int j=0;j<3;j++){
            printf("Enter %d and %d th element of matrix B: \n",i,j);
            scanf("%d",&matrixB[i][j]);
        }
    }
matrixmulAB[0][0]=matrixA[0][0]*matrixB[0][0]+matrixA[0][1]*matrixB[1][0]+matrixA[0][2]*matrixB[2][0];
matrixmulAB[0][1]=matrixA[0][0]*matrixB[0][1]+matrixA[0][1]*matrixB[1][1]+matrixA[0][2]*matrixB[2][1];
matrixmulAB[0][2]=matrixA[0][0]*matrixB[0][2]+matrixA[0][1]*matrixB[1][2]+matrixA[0][2]*matrixB[2][2];
matrixmulAB[1][0]=matrixA[1][0]*matrixB[0][0]+matrixA[1][1]*matrixB[1][0]+matrixA[1][2]*matrixB[2][0];
matrixmulAB[1][1]=matrixA[1][0]*matrixB[0][1]+matrixA[1][1]*matrixB[1][1]+matrixA[1][2]*matrixB[2][1];
matrixmulAB[1][2]=matrixA[1][0]*matrixB[0][2]+matrixA[1][1]*matrixB[1][2]+matrixA[1][2]*matrixB[2][2];
matrixmulAB[2][0]=matrixA[2][0]*matrixB[0][0]+matrixA[2][1]*matrixB[1][0]+matrixA[2][2]*matrixB[2][0];
matrixmulAB[2][1]=matrixA[2][0]*matrixB[0][1]+matrixA[2][1]*matrixB[1][1]+matrixA[2][2]*matrixB[2][1];
matrixmulAB[2][2]=matrixA[2][0]*matrixB[0][2]+matrixA[2][1]*matrixB[1][2]+matrixA[2][2]*matrixB[2][2];
 for(int i=0;i<3;i++){
        for(int j=0;j<3;j++){
            printf("%d\t",matrixmulAB[i][j]);
            if(i==0&&j==2){
                printf("\n");
            }
            if(i==1&&j==2){
                printf("\n");
            }
            if(i==2&&j==2){
                printf("\n");
            }
        }
    }

}
