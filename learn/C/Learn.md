# 基本概念

## 1.Hello, World!

```c
#include <stdio.h>

int main() {
  printf("Hello, World!\n");
  return 0;
}
```

## 类型

```
int： 整数。%d
float：浮点数，带小数的数字。%f
double：双精度浮点值。
char：单个字符。每种类型所需的存储量因平台而异。%c
```


变量 必须以字母或下划线开头,可以由字母，数字和下划线字符组成

常量

- 在变量声明中使用**const** `const double PI = 3.14;`
- 使用#define预处理程序指令 `#define PI 3.14` 

```c
//d 十进制 ％ld 格式说明符 c 字符 s 字符串 f 浮点数 e 科学计数法 x 十六进制
printf("Color: %s, Number: %d, float: %5.2f \n", "red", 42, 3.14159);
```

## 输入输出

1. 输入

```
char a = getchar();
printf("你输入: %c", a);
```

> 仅单字符串





# 输入项

C支持多种方式来接受用户输入。
**getchar（）**返回下一个单个字符输入的值。

**例如**：

```c
#include <stdio.h>

int main() {
    char a = getchar();

    printf("You entered: %c", a);

    return 0;
}
```

输入存储在变量**a中**。 的**获取（）**函数是用来读输入为有序的字符序列，也被称为**串**。 字符串存储在char数组中。

```c
#include <stdio.h>

int main() {
    char a[100];

    gets(a); 

    printf("You entered: %s", a);

    return 0;
}
```

在这里，我们将输入存储在100个字符的数组中。 **scanf（）**扫描与格式说明符匹配的输入。

```c
#include <stdio.h>

int main() {
    int a;
    scanf("%d", &a);

    printf("You entered: %d", a);

    return 0;
}
```

在**与**变量名前标志是**地址运算符**。它给出了变量的地址或在内存中的位置。这是必需的，因为**scanf**将输入值放置在变量地址上。 作为另一个示例，让我们提示输入两个整数输入并输出它们的和：

```c
#include <stdio.h>

int main() {
    int a, b;
    printf("Enter two numbers:");
    scanf("%d %d", &a, &b);

    printf("\nSum: %d", a+b);

    return 0;
}
```

>  **scanf（）**遇到空格后立即停止读取，因此“ Hello World”之类的文本是**scanf（）的**两个单独输入。

# 输出

在前面的课程中，我们已经使用过**printf（）**函数生成输出。在本课程中，我们将介绍可用于输出的其他几个功能。 **putchar（）**输出单个字符。

```c
#include <stdio.h>
int main() {
  char a = getchar();
  printf("You entered: ");
  putchar(a);
  return 0;
}
```

输入存储在变量**a中**。 该**puts（）**函数是用来显示输出作为**字符串**。 字符串存储在char数组中。

```c
#include <stdio.h>

int main() {
  char a[100];

  gets(a); 

  printf("You entered: ");
  puts(a); 

  return 0;
} 
```

在这里，我们将输入存储在100个字符的数组中。 **scanf（）**扫描与格式说明符匹配的输入。

```c
#include <stdio.h>

int main() {
    int a;
    scanf("%d", &a);

    printf("You entered: %d", a);

    return 0;
}
```

在**与**变量名前标志是**地址运算符**。它给出了变量的地址或在内存中的位置。这是必需的，因为**scanf**将输入值放置在变量地址上。 作为另一个示例，让我们提示输入两个整数输入并输出它们的和：

```c
#include <stdio.h>

int main() {
    int a, b;
    printf("Enter two numbers:");
    scanf("%d %d", &a, &b);

    printf("\nSum: %d", a+b);

    return 0;
}
```

>  **scanf（）**遇到空格后立即停止读取，因此“ Hello World”之类的文本是**scanf（）的**两个单独输入。


