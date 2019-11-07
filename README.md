#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

char* input;
int* flag;
int isEmpty = 1;
int cnt = 0;
char fname[20];
FILE* fp;

void printIdx(int cnt) {
	int cipher = 1;
	char num[5] = "0000";
	sprintf(num, "%d", cnt);
	char s[10] = "[0000]";
	int temp = cnt;
	int idx = 0;

	while (temp / 10 >= 1) {
		cipher++;
		temp /= 10;
	}
	for (int i = 1; i < 5; i++) {
		if (i < 5 - cipher)
			s[i] = '0';
		else {
			s[i] = num[idx];
			idx++;
		}
	}
	printf("%s ", s);
	fprintf(fp, "%s ", s);
}
