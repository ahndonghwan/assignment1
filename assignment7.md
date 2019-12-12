#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
#include <stdlib.h>
#include <string.h>


int main(int argc, char* argv[]) {

	FILE* fp1, * fp2;
	char str[5];   
	if ((fp1 = fopen(argv[1], "input2")) == NULL) { 
		printf("fale to open file.");
		return 0;
	}
	if ((fp2 = fopen(argv[2], "output2")) == NULL) { 
		printf("fail to create file for write.");
		return 0;
	}
	int nNumber = 0;


	int toknum = 0;
	char src[] = "Hello,, world!";
	const char delimiters[] = ", !";
	char* token = strtok(src, delimiters);
	while (token != NULL)
