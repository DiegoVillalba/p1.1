# p1.1
1.
#include<stdio.h>
int temp,j,i,k;
int lista[10]={25,69,8,5,1,4,7,50,90,10};
int tamanolista=10;
int main(){
	for (i=0;i<tamanolista-1;i++){
		for(j=0;j<tamanolista-1;j++){
			   if(lista[j]>lista[j+1]){
			   	    temp=lista[j];
			   	    lista[j]=lista[j+1];
			   	    lista[j+1]=temp;
			   }
		}
	}
	for(k=0;k<tamanolista;k++){
		printf("%i   ",lista[k]);
	}
}
