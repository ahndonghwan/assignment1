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

while (token != NULL)
	{
		printf("%d: [%s]\n", ++toknum, token);
		token = strtok(NULL, delimiters);

		char string[100];


fputs(" ^ ^^^^^^^^^^^^^^\n", fp2);
	fputs("Dong Hwan Ahn\n", fp2);
	fputs("Student ID : 2018120116\n", fp2);
	fputs("^^^^^^^^^^^^^^^\n", fp2);
	

	fclose(fp1);
	fclose(fp2);
	return 0;
}
