#pragma warning(disable:4996)

#include <stdio.h>
#include <stdlib.h>

struct personscore {
	int num;
	char nme[10];
	float scr;
	float scr2;
};

typedef struct personscore psc;

psc ps;
psc* pps = &ps;