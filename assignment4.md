#assignment4

#include <stdio.h>

int modify_data[10] = { 1,2,3,4,5,6,7,8,9,10 };

void powerset(int n)
{
	int i, j;
	int max = 1 << n;
	for (i = 0; i < max; i++) {
		if (i == 0)
			printf("[%c",155);
		else
		printf("[");
		for (j = 0; j < n; j++) {
			if (i & (1 << j)) printf("%d", modify_data[j]);
		}
		printf("]\n");
		
	}
	{printf("^^^^^^^^^^^^^^^\n");
	printf("Dong Hwan Ahn\n");
	printf("Student ID : 2018120116\n");
	printf("^^^^^^^^^^^^^^^\n");
	}
}

int main()
{
	powerset(sizeof(modify_data) / sizeof(int));
	return 0;
}

#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>

int main(int argc, char* argv[]) {

	FILE* fp1, * fp2;
	char str[64];   // change the number appropriately to your program
	// read_file = argv[1]
	// write_file = argv[2]
	int modify_data[10] = { 1,2,3,4,5,6,7,8,9,10 };

	void powerset(int n);
	{
		int i, j;
		int max = 1 << n;
		for (i = 0; i < max; i++) {
			if (i == 0)
				printf("[%c", 155);
			else
				printf("[");
			for (j = 0; j < n; j++) {
				if (i & (1 << j)) printf("%d", modify_data[j]);
			}
			printf("]\n");

		}
		{printf("^^^^^^^^^^^^^^^\n");
		printf("Dong Hwan Ahn\n");
		printf("Student ID : 2018120116\n");
		printf("^^^^^^^^^^^^^^^\n");
		}
	}