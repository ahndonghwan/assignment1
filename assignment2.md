#include <stdio.h>

int main(void) {
	int num1 = 0;
	int num2 = 0;
	int value = 0;
	char a = 0;

	printf("���� �Է��Ͻÿ� : ");
	scanf("%d %c %d", &num1, &a, &num2);

	switch (a) {
	case '+':
		value = num1 + num2;
		printf("%d",value);
		printf("%s", " \n^^^^^^^^^^^^^^^^^\n 2018120116 dong hwan ahn \n^^^^^^^^^^^^^^^");
		break;
	case '-':
		value = num1 - num2;
		printf("%d",value);
		printf("%s", " \n^^^^^^^^^^^^^^^^^\n 2018120116 dong hwan ahn \n^^^^^^^^^^^^^^^");
		break;
	}
		return 0;
	}