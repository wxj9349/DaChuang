1. 严格执行缩进，缩进为4个空格，（可使用插件来格式化代码）
2. 右括号所在的行不能有其它东西，包括注释（do-while语句除外）
3. 一行只写一条语句
```
错误示例：int a = 0; double b = 0;
```
4. if, for, while等语句的执行语句部分无论多少都要加花括号
```
if(a > 0)
{
    a++;
}
```
5. 关于空格，如下
```
for (int i = 0, b = 0; i < 10, b < 10; i++, b++)
{
    *p = a;
    p->id = num;
    p = &b;
    a = b ^ 2;
}
```
6. 避免分散定义变量，尽量在文件首部位置
7. 同一行不要定义过多变量
```
错误示例：int a, b, c, d, e;
```
8. 定义的变量，能初始化的必须初始化
```
int a = 0;
double b = 0;
float c = 0;
char d = "";
string e = "";
bool f = false;
int nums[5] = {0};
```
9.变量名用帕斯卡命名法，不要用a,b,c,d这种无法表示含义的（循环中的临时变量除外）
```
string UserName
```
10. 函数名用帕斯卡命名法
```
string GetName(){}
void ShowPasswordAndUsername(){}
```
11.  写代码的文件夹已经创建好，在Assets/ExternalFiles/RandomNum/Code.c里写代码，生成的数据放在Assets/ExternalFiles/RandomNum/TxtFolder文件夹里