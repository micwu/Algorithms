#include <stdio.h>
#include <stdlib.h>
#include <assert.h>
#include <string.h>

#define true 1
#define false 0
char* strStr1(const char* str, const char* target);

char* strStr(const char* str, const char* target)
{
	if (!*target) return str;
	char *p1 = (char *)str;

	while (*p1)
	{
		char *p1begin = p1;
		char *p2 = (char *)target;
		while (*p1 && *p2 && (*p1 == *p2))
		{
			p1++;
			p2++;
		}
		if (!*p2) return p1begin;
		p1++;
	}
	return NULL;
}

int main()
{
	char a[] = "abcdef";
	//char b[] = "df";
	char b[] = "f";
	char* targ = strStr(a, b);
		printf("%s\n", targ);
	
	char* str = strStr1(a, b);
		
	printf("%s\n",str);
		
	system("pause");
}

char* strStr1(const char* str, const char* target)
{
	int i, j;
	int n = strlen(str);
	int m = strlen(target);
	char *p1 = (char*)str;
	for (i = 0, j = 0; i != n; i++)
	{		
		if (str[i] == target[j])
		{
			j++;
		}
		else
		{
			j = 0;
		}
		if (j == m)
			return (p1+i-j+1);
	}
}
