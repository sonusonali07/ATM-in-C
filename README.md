#include<stdio.h>
int insertElement(int arr[],int key,int n,int capacity){
    if(n>=capacity){
        return n;
    }
    arr[n]=key;

    return n+1;
}
int main(){
    int arr[20]={1,2,7,5,3,4};
    int capacity=sizeof(arr)/sizeof(int);
    int i ,key=77, n=6;
    
    printf("\n Before Insertion: ");
    for (i = 0; i < n; i++)
        printf("%d  ", arr[i]);
 
    // Inserting key
    n=insertElement(arr,key,n,capacity);
 
    printf("\n After Insertion: ");
    for (i = 0; i < n; i++)
        printf("%d  ",arr[i]);
 
    return 0;
}
