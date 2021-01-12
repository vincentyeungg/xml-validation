#include <stdio.h>
#include <stdlib.h>
#include <ctype.h>
extern int pop();
extern void push(int);
extern int isEmpty();

int main(int argc, char * argv[])
{
  int ch,poped;
  while ((ch = getchar()) != EOF) {
    if (!(isalpha(ch) || ch == '>' || ch == '<' || ch == '/'))
      continue;
	else if(ch=='<'){
		ch  = getchar();
			if ((isalpha(ch))){
				push(ch);}
			else if(ch == '/'){
				ch  = getchar();
				if(isEmpty()){
					exit(0);}
				poped = pop();
				if(poped != ch){
					printf("NOT Valid!!!!!\n");
					exit(1);
				}
			}
		} 
	}
	if(!(isEmpty())){
		printf("NOT Valid\n");
		exit(1);}
	else{
		printf("Valid\n");
		exit(0);}
    
  }


