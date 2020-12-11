#include <stdio.h>
#include <stdlib.h>
#define N 5
int queue[N];
void enq(int a,int *front,int *rear){
if(*rear==N-1)
  printf("\n QUEUE IS FULL");
else {
  if(*front ==-1)
    *front=0;
  (*rear)++;
  queue[*rear]=a;
  printf("\n Insertion Done!");}}

void deq(int *front ,int *rear){
if(*front==*rear)
  printf("\n QUEUE is empty");
else {
  printf("\n deleted element %d",queue[*front]);
  *front=*front+1;
}}

void display(int *front,int *rear){
if(*rear==-1)
  printf("\n QUEUE IS EMPTY!!");
else{int i;
  printf("\n QUEUE elements are :\t");
  for(i=*front ;i<=*rear;i++)
    printf("%d\t",queue[i]);}}

int main(){
int a,choice;
int *front=-1,rear=-1;
while(1){
  printf("\n ENTER \n");
  printf(" 1.TO INSERT");
  printf("\n 2.TO DELETE");
  printf("\n 3.TO DISPLAY");
  printf("\n 4.TO EXIT");
  printf("\n Enter your choice");
  scanf("%d",&choice);
  switch(choice){
case 1:
  printf("Enter the value to inset");
  scanf("%d",& a);
  enq(a,&front,&rear);
  break;
case 2:
  deq(&front,&rear);
  break;
case 3:
  display(&front,&rear);
  break;
case 4:
  return 0;
default:
  printf("\n INVALID ");
  }
}
return 0;
}
