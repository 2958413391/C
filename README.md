# C
zixue
#define _CRT_SECURE_NO_WARNINGS 1
#define _CRT_SECURE_NO_WARNINGS 1
#include<stdio.h>
#include<string.h>
//scanf - 输入
//int main()
//{
//	int num1 = 0;
//	int num2 = 0;
//    int sum = 0;
//	scanf("%d%d", &num1, &num2);
//	/*scanf
//	strcpy
//    strlen
//    stract*/
//	sum = num1 + num2;
//printf("sum = %d\n", sum);
//	return 0;
//} 

//常量 
//int main()
//{
	//const - 常属性
	// const int n =10;
	// int arr[n] = {0};
	 //n =20;
	//const修饰的常变量
	//const int num = 4;
	//printf("%d\n", num);
	//num = 8;
	//printf("%d\n", num);
	//return 0;
	//3;//字面常量
//}

////#define定义的标识符常量
////标识符常量 - 它是指用一个符号来代替一个数值
//#define MAX 10
//int main()
//{
//	int arr[MAX] = { 0 };
//	printf("%d\n", MAX);
//	return 0;
//}

////枚举常量
////枚举 - 一一例举
////枚举关键字 - enum
//enum Sex
//{
//	MALE,
//	FEMALE, 
//	SECRET
//};
//  //MALE,FEMALE,SECRET - 枚举常量
//int main()
//{
//	//enum Sex s = FEMALE;
//	/*枚举加上枚举名，可以用作参数，来限制参数传入的内容
//		相当于是一种代码规范化的限制，因为大家都喜欢用 int 来表示各种 type
//		但是对于一个函数如何限制使用者只能传入合法的数值呢？那就用枚举并定义枚举名
//		不加枚举名也是可以定义枚举的，比如
//		enum {
//		MALE,
//		FEMALE,
//		SECRET,
//	};
//	这样的枚举其实和C中的宏定义类似
//        #define MALE (0)
//        #define FEMALE (1)
//        #define SECRET (2)*/
//		
//	printf("%d\n", MALE);//0
//	printf("%d\n", FEMALE);//1
//	printf("%d\n", SECRET);//2
//
//	return 0;
//}

//字符串
//int main()
//{
//	"abcde";
//		"";//空字符串 
//		return 0;
//}
//int main()
//{
//	//数据中在计算机上储存的时候，储存的是二进制
//	//a=97
//	//A=65
//	//ASCII编码
//	//ASCII码值
//
//	char arr1[] = "abc";//数组
//	//"abc"-- 'a' 'b' 'c' '\0'   '\0'--字符串的结束标志
//	char arr2[] = { 'a','b','c','\0'};
//	//'a' 'b' 'c' 
//	printf("%s\n", arr1);
//	printf("%s\n", arr2);
//	return 0;
//}
//int main()
//{
//	char arr1[] = "abc";
//	char arr2[] = { 'a','b','c',0};
//	printf("%d\n", strlen(arr1));//strlen - string length - 计算字符串长度的
//	printf("%d\n", strlen(arr2));
//	return 0;
//}

//转义字符
//int main()
//{
//	printf("abc\n");
//	return 0;
//}
//int main()
//{
//	printf("nihao\\tt");
//	//\t - 水平制表符
//     printf("%c\n", '\'');
//	 printf("%s\n", "\"");
//		return 0;
//}
//int main()
//{
//	printf("%d\n", strlen("c:\test\32\test.c"));
//	//\32 -- 32是2个8进制数字
//	//32作为8进制代表的那个十进制数字，作为ASCII码值，对应的字符
//	//32转换为十进制  =26  作为ASCII码值代表的字符
//	printf("%c\n", '\132');
//	printf("%c\n", '\x61');
//	return 0;
//}

//选择语句
//int main()
//{
//	int input = 0;
//	printf("你会好好听小蒲的话吗？（1 or 0）:>");
//	scanf("%d", &input);//1/0
//	if (input == 1)
//		printf("会\n");
//	else
//		printf("不会\n");	
//	return 0;
//	}

//循环语句
//int main()
//{
//	int line = 0;
//	printf("喜欢小蒲多久？\n");
//
//	while (line < 10000)
//	{
//		printf("喜欢一辈子:%d\n", line);
//		line++;
//	}
//	if (line >= 10000)
//		printf("小蒲是你的了\n");
//	return 0;
//}

//函数
	 //定义函数
//int Add(int x, int y)
//{
//	int z = x + y;
//	return z;
//}
//int main()
//{
//	int num1 = 10;
//	int num2 = 20;
//    int sum = 0;
//	int a = 100;
//	int b = 200;
//;   //sum = num1 + num2;
//    sum = Add(num1 , num2);
//    //sum = a + b;
//    sum = Add(a, b);
//printf("sum = %d\n", sum);
//	return 0;
//}

//数组
//int main()
//{
//	int arr[10] = { 1,2,3,4,5,6,7,8,9,10 };//定义一个存放10个整数数字的数组
//	//0-9
//	int i = 0;
//	while (i < 10)
//	{
//		printf("%d ", arr[i]);
//		i++;
//	}
//	
//	//printf("%d\n", arr[4]);//下标的方式访问元素    
//	//arr[下标]
//	//char ch[20];
//	//float arr2[5];
//	return 0;
//}

//操作符
// 算术
//int main()
//{
//	int a = 5%2;//取模
//	printf("%d\n", a);
//	return 0;
//}
//int main()
//{
// 移位
//	//移（2进制）位操作符
//	//<<左移
//	//>>右移
//	int a = 1;
//	//整型1占4个字节-32个比特位
//	//00000000000000000000000000000001
//	/*int b = a << 1;//2
//	printf("%d\n", b);*/
//	int b = a << 2;//4
//	printf("%d\n", b);
//	printf("%d\n", a);//1
//	return 0;
//}
//位
//int main()
//{
//	//(2进制）位操作
//	//  &   按位与   计算规律  0为假，1为真  一假则假
//	//  |   按位或             一真为真
//	//  ^   按位异或           对应的二进制位相同，则为0； 不同，则为1
//	int a = 3;   //  011
//	int b = 5;   //  101
//	int c = a & b;  //  001  
//	int c = a | b;  //  111
//	int c = a ^ b;  //  110
//	printf("%d\n", c);
//	return 0;
//}
//赋值
//int main()
//{
//	int a = 10;
//	a = 20;// = 赋值    ==  判断相等
//	a = a + 10;
//	a += 10;
//	a = a - 20;
//	a -= 20;
//	a = a & 2;
//	a &= 2;
//	//复合赋值符
//	// = += -= *= /= &= ^=  |=    >>=   <<=
//	return 0;
//}
//单目操作符
//int main()
//{
//	//C语言中表示真假
//	// 0-假
//	//非0-真
//	int a = 10;
//	int a = -2;//-
//	printf("%d\n", a);
//	printf("%d\n", !a);//!
//	//sizeof 计算的是变量/类型所占空间大小，单位为字节
//	printf("%d\n",sizeof(a));//4字节  写法1
//	printf("%d\n", sizeof(int));//  写法2
//	printf("%d\n", sizeof a);//  写法3
//	//计算数组
	//int arr[10] = { 0 };//10个整型元素的数组
	//int sz = 0;
//	//10*sizeof(int) = 40
	//printf("%d\n", sizeof(arr));
//	//计算数组的元素个数
//	//个数 = 数组总大小/每个元素大小
//	sz = sizeof(arr) / sizeof(arr[0]);
//	printf("%d\n", sizeof(arr)/sizeof(arr[0]));
//	printf("sz = %d\n", sz);
//return 0;
//}
//int main()
//{
//	int a = 0;//4个字节，32个比特位
//	int b = ~a;//b是有符号的整型
//	// ~ --按（2进制）位取反
//	//  00000000000000000000000000000000
//	//  11111111111111111111111111111111
//	// 源码，反码，补码
//	// 负数在内存中存储的时候，储存的是二进制的补码
//	//1010
//	//0101
//	printf("%d\n", b);//使用的，打印的是这个数的源码
//	return 0;
//}
//int main()
//{
//	int a = 10;
//	//int b = a++;//后置++，先使用，后++  11,10
//	//int b = ++a;//前置++，先++，后使用  11,11
//	//int b = a--;//后置--，先使用，后--  9,10  
//	//int b = --a;//前置--，先--，后使用  9.9
//	printf("a = %d b = %d\n", a, b);
//	return 0;
//}
//int main()
//{
//	int a = (int)3.14;//强制类型转换
//	return 0;
//}
//int main()
//{
//	//真  -非0
//	//假  - 0
//    //&&  - 逻辑与
//	//||  - 逻辑或
//	int a = 0;
//	int b = 3;
//	int c = a && b;
//	int c = a || b;
//	printf("c = %d\n", c);
//	return 0;
//}
// 条件操作符
//三目操作符
//int main()
//{
//	int a = 10;
//	int b = 20;
//	int max = 0;
//	max = (a > b ? a : b);
//	/*if (a > b)
//		max = a;
//	else
//		max = b;*/
//	printf("max = %d\n", max);
//	return 0;
//}
//int main()
//{
//	int arr[10] = { 0 };
//	arr[4];// [] - 下标引用操作符
//	return 0;
//}
// int Add(int x, int y)
//{
//	int z = x + y;
//	return z;
//}
//int main()
//{
//	int num1 = 10;
//	int num2 = 20;
//    int sum = 0;
//    sum = Add(num1 , num2);//() - 函数调用操作符
//printf("sum = %d\n", sum);
//	return 0;
//}
//双目操作符
//三目操作符
//int main()
//{
//	int a = 10;
//	int b = 20;
//	a + b;// +  两个操作数   双目操作符
//	return 0;
//}

//关键字
//int main()
//{
//	auto int a = 10;//局部变量- 自动变量  auto一般被省略
//	return 0;
//}
//int main()
//{
//	//register int a = 10;//建议把a定义成寄存器变量
//	int a = 10;
//	a = -2;
//	//int 定义的变量是有符号的
//	//signed int;//signed通常被省略
//	//unsigned 定义无符号变量
//	return 0;
//}
//int main()
//{
////typedef - 类型定义 - 类型重定义
//	typedef unsigned int num u_int;
//	unsigned int num = 20;
//	u_int num 2 = 20;
//	return 0;
//}
//static 修饰局部变量
//局部变量的生命周期变长
//void test()
//{
//	static int a = 1;//a 是一个静态的局部变量
//	a++;
//	printf("a= %d\n", a);
//}
//int main()
//{
//	int i = 0;
//	while (i < 5)
//	{
//		test();
//		i++;
//	}
//	return 0;
//}
//static 修饰全局变量
//改变了变量的作用域 - 让静态的全局变量只能在自己所在的源文件内部使用
//出了源文件无法使用
//int main()
//{
//	//extern - 生命外部符号
//	extern int g_val;
//	printf("g_val= %d\n", g_val);
//	return 0;
//}
//static修饰函数
//static修饰函数改变了函数的链接属性
// 外部链接属性改变为内部链接属性 
//声明外部函数
//extern int Add(int, int);
//int main()
//{
//	int a = 10; 
//	int b = 20;
//	int sum = Add(a, b);
//	printf("sum = %d\n", sum);
//	return 0;
//}
//#define定义标识符常量
//#define MAX 100
//int main()
//{
//	int a = MAX;
//	return 0;
//}
//#define 可以定义宏- 带参数
//函数的实现
//int Max(int x, int y)
//{
//	if (x > y)
//		return x;
//	else
//		return y;
//}
////宏的定义
//#define MAX(X,Y) (X>Y?X:Y)
//int main()
//{
//	int a = 10;
//	int b = 20;
//	//函数
//	int max = MAX(a, b);
//	printf("max = %d\n", max);
//	//宏的方式
//	max = MAX(a, b);
//	printf("max = %d\n", max);
//	return 0;
//}
//int main()
//{
//	int a = 10;//4个字节
//	//&a;//取地址
//	int* p = &a;//取地址
//	//printf("%p\n", &a);
//	//printf("%p\n", p);
//	*p = 20;//* - 解引用操作符
//	printf("%p\n", p);
//	//有一种变量是用来存放地址的 - 指针变量
//	//printf("%p\n", &a);
//	return 0;
//}
//int main()
//{
//	char ch = 'w';
//	char* pc = &ch;
//	*pc = 'a';
//	printf("%c\n", ch);
//	return 0;
//}

//结构体
//复杂对象 - 结构体 - 自己创造的一种类型
//创建一个结构体变量
//struct Book
//{
//	char name[20];//C语言程序设计
//	short price;//55
//};
//int main()
//{
//	//利用结构体类型-创建一个该类型的结构体变量
//	struct Book b1 = { "C语言程序设计", 55 };
//	strcpy(b1.name, "C++");//strvpy-string copy -字符串拷贝- 库函数-string.h
//	printf("%s\n", b1.name);
//	struct Book* pb = &b1;
//	//利用pb打印出我的书名和价格
//	//    结构体变量.成员
//	//    结构体变量->成员
//	printf("书名:%s\n", pb->name);
//	printf("价格:%d元\n", pb->price);
//	/*printf("书名:%s\n", (*pb).name);
//	printf("价格:%d元\n", (*pb).price);*/
//	/*printf("书名:%s\n", b1.name);
//	printf("价格:%d元\n", b1.price);
//	b1.price = 15;
//	printf("修改后的价格:%d元\n", b1.price);*/
//	return 0;
//}
