#define _CRT_SECURE_NO_WARNINGS 1
#include <stdio.h>
//结构体
//一个复杂对象，结构体来描述，是自己创造出来的类型
struct Book
{
	char name[20];//c语言程序设计
	short price;//55 价格
};
int main()
{
	struct Book b1=
	{
		"c语言程序设计",55
	};
	struct Book* pb = &b1;
	//利用pb打印书名和价格
	printf("%s\n", pb->name);
	printf("%d\n", pb->price);
	//.  结构体变量.成员
	//->  结构体指针->成员

	/*printf("书名:%s\n", b1.name);
	printf("价格:%d元\n", b1.price);*/
	return 0;
}
//int main()
//{
//	double d = 3.14;
//	double* pd = &d;
//	printf("%d\n", sizeof(pd));
//	/**pd=5.9;
//	printf("%lf\n", d);*/
//	//int a = 10;//申请了4个字节的空间
//	////printf("%p\n", &a);
//	//int* p = &a;//p是一个变量，如果用来存放地址，则称p为指针变量
//	////printf("%p\n", p);
//	//*p=20;//解引用操作符，或者叫间接访问操作符,把a赋值20
//	//printf("%d\n", a);
//	return 0;
//}
