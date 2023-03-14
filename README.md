# Ytai
#include<stdio.h>


//typedef struct stu//定义一个结构体类型
//{
//	//描述一个学生
//	char name[20];
//	short age;
//	char phone[20];
//	char sex[5];
//}stu;
//
//
//int main()
//{
//	struct stu s = { "张三",20,"15926964871","男" };//创建结构体变量
//	return 0;
//}





//struct s
//{
//	int a;
//	char c;
//	char arr[20];
//	double d;
//};
//
//
//struct T
//{
//	char ch[10];
//	struct s s1;
//	char* pc;
//};
//
//
//
//int main()
//{
//	char arr[] = "hello";
//		struct T t = { "hehe",{100,'b',"hello",3.14},arr };
//	return 0;
//}





typedef struct stu//定义一个结构体类型
{
	//描述一个学生
	char name[20];
	short age;
	char phone[20];
	char sex[5];
}stu;


void Print(stu s)
{
	printf("name: %s\n", s.name);
}


void Print2(stu* ps)
{
	printf("name: %s\n", ps->name);
}

int main()
{
	struct stu s = { "张三",20,"15926964871","男" };
	Print(s);
	Print2(&s);
	return 0;
}
