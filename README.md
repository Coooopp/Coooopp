struct Book
{
	char name[20];
	short price;
};

int main()
{

	struct Book b1 = {"C语言程序设计",55};
printf("书名:%s\n", b1.name);
printf("价格:%d元\n", b1.price);
	return 0;
}


include<stdio.h>

int main()
{
	int a = 10;

	printf("%p\n", &a);
	
	return 0;
}
int main()
{
	int a = 10;
	int *p = &a;//指针 用于存放地址的一种方法，方便快捷。
	printf("%p\n", &a); 
	printf("%p\n", p);
	return 0;
}
int MAX(int x, int y)
{
	if (x > y)
		return x;
	else
		return y;
}
int main()
{
	int a = 20;
	int b = 30;
	int max = MAX(a, b);
	printf("max =%d\n ", max);
	return 0;
}
static int Add(int x, int y)
{
	int z = x + y;
	return z;
}
int main ()
{
	int a = 50;
	int b = 70;
	int sum = Add(a,b);
	printf("sum=%d\n", sum);

	return 0;
}
void test ()
{
	static int a = 1;//static 修饰局部变量
	a++;
	printf("a=%d\n", a);
}
int main()
{
	int i = 0;
 	while (i < 5)
	{
		test();
		i++;
	}

	return 0;
	
	#include <stdio.h>

int main()
{
	int i = 1;
	while (i<=100)
	{
		if (i % 2 == 1)
			printf("%d ", i);
		i++;
	}
	return 0;
}\\判断0到100数的奇数
int main()
{
	int i;
	scanf_s("%d", &i);
	if (i % 2 == 1)
	{
		printf("这个数是奇数");
	}
	else
		printf("这个数不是奇数");
	return 0;
}//判断一个数是奇数

