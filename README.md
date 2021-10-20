#define _CRT_SECURE_NO_WARNINGS 1

#include<stdio.h>

#include<string.h>

#define MAX(X,Y) (X > Y ? X : Y)

int Max(int x, int y)

{

	int z = x + y;
  
	return z;
  

}


struct Book

{

	char name[20];
  
	short price;
  
};


int main()

{



	struct Book b1 = { "C程序设计",55 };
  
	printf("书名：%s\n", b1.name);
  
	printf("价格：%d\n", b1.price);
  


	char ch = 'w';
  
	char *pc = &ch;
  
	*pc = 'a';
  
	printf("%c\n", ch);
  

	int a = 10;
  
	int *p = &a;
  
	*p = 20;
  
	printf("%p\n", &a);
  
	printf("%p\n", p);
  
	printf("a=%d\n", a);
  

	int a = 10;
  
	int b = 20;
  
	int max = Max(a, b);
  
	printf("max=%d\n", max);
  
	max = MAX(a, b);
  
	printf("max=%d\n", max);
  

	int month;
  
	printf("请输入：\n");
  
	scanf("%d", &month);
  
	switch (month)
  
	{
  
	case 1:
  
	case 2:
  
	case 3:
  
	case 4:
  
	case 5:
  
	{
  
		printf("工作日\n");
    
	     break;
       
	}
  
	case 6:
  
	case 7:
  
	{
  
		printf("休息日\n");
    
		break;
    
	}
  
	}
  
	return 0;
  
}
