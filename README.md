# PTA_7-12
# 两个数的简单计算器
# 本题要求编写一个简单计算器程序，可根据输入的运算符，对2个整数进行加、减、乘、除或求余运算。题目保证输入和输出均不超过整型范围。

# 输入格式：输入在一行中依次输入操作数1、运算符、操作数2，其间以1个空格分隔。操作数的数据类型为整型，且保证除法和求余的分母非零。

# 输出格式：当运算符为+、-、*、/、%时，在一行输出相应的运算结果。若输入是非法符号（即除了加、减、乘、除和求余五种运算符以外的其他符号）则输出ERROR。
```cpp
#include<iostream>
using namespace std;
int main() {  //很简单，也可以用switch-break语句来做
	int a, b;
	char op;
	cin >> a >> op >> b;
	if (op == '+') {
		cout << a + b;
	}
	else if (op == '-') {
		cout << a - b;
	}
	else if (op == '*') {
		cout << a * b;
	}
	else if (op == '/') {
		cout << a / b;
	}
	else if (op == '%') {
		cout << a % b;
	}
	else {
		cout << "ERROR";
	}
	return 0;
}