[SoloLearn-c](https://www.sololearn.com/Play/C)
# 基本概念

## 1.Hello, World!

```
#include <stdio.h>

int main() {
  printf("Hello, World!\n");
  return 0;
}
```
## 类型
```
int： 整数。
float：浮点数，带小数的数字。
double：双精度浮点值。
char：单个字符。
```
变量 必须以字母或下划线开头,可以由字母，数字和下划线字符组成

常量 
- 在变量声明中使用**const** `const double PI = 3.14;` [1618](https://code.sololearn.com/1618/#c)
- 使用#define预处理程序指令 `#define PI 3.14` [1635](https://code.sololearn.com/1635/#c)

## 输入输出
1. 输入
```
char a = getchar();
printf("你输入: %c", a);
```
> 仅单字符串



# %d
```
printf("Color: %s, Number: %d, float: %5.2f \n", "red", 42, 3.14159);
```
d 十进制 
％ld 格式说明符
c 字符 
s 字符串 
f 浮点数 
e 科学计数法 
x 十六进制
[参考](https://code.sololearn.com/1650/#c) [2](https://www.sololearn.com/Play/C)

