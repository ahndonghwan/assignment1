#assignment4.1

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
	// see the usage of r, rt, w, wt, r+, w+
	if ((fp1 = fopen(argv[1], "r")) == NULL) { //fail to open file for read
		printf("fale to open file.");
		return 0;
	}
	if ((fp2 = fopen(argv[2], "wt")) == NULL) { //fail to open file for write
		printf("fail to create file for write.");
		return 0;
	}

	while (fgets(str, sizeof(str), fp1)) {   // read a file and write to another file line by line
		printf("%d\n", str);
		fputs(str, fp2);
	}

	fclose(fp1);
	fclose(fp2);
	return 0;
}