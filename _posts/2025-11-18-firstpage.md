---
layout: post
title: 第一篇博客
---

# 1. 命名方法
## 1.1 驼峰命名法
指混合使用大小写字母来构成变量和函数的名字。当变量名或函数名是由一个或多个单词连结在一起构成的唯一识别字时，第一个单词以小写字母开始，从第二个单词开始以后的每个单词的首字母都采用大写字母，例如：myName、myAge，这样的变量名看上去就像骆驼峰一样此起彼伏，因此被称为驼峰命名法。

``` Cpp
int *treeBase;
int elemNum;
int treeSize;
```
## 1.2  帕斯卡（Pascal）命名法
也叫大驼峰法，与驼峰命名法类似，不过骆驼命名法是首字母小写，而帕斯卡命名法是首字母大写。

```Cpp
int *TreeBase;
int ElemNum;
int TreeSize;
```
## 1.3 匈牙利命名法
臃肿不推荐

## 1.4 下划线命名法
与驼峰命名法相似，通过一种方式将不同单词区分开，方便读懂变量含义。与驼峰命名法不同的是，驼峰命名法采用的是首字母大写区分，下划线命名法是在不同单词之间添加下划线。

```cpp
int *tree_base;
int elem_num;
int tree_size;
```

# 2. windows下C++命名规范
对于C++固有类型，如类，函数，他们有各自的命名规则，当然不同公司有不同公司的命名要求，在这里说一下大多数要求，大家作为了解。

## 2.1 1、类与对象的命名
类的名称一般以大写字母“C”开头，表明定义的是类，后跟一个或多个单词。为便于界定，每个单词的首字母要大写。类的命名推荐用"名词"或"形容词＋名词"的形式。

```Cpp
class CPerson;
 
class CLittleCat;
```
## 2.2 函数命名
函数的名称由一个或多个单词组成。为便于界定，建议采用帕斯卡（Pascal）命名法，即每个单词的首字母要大写。

```cpp
int InitQueue(LinkQueue &LQ) ;
 
int EnQueue(LinkQueue &LQ, int e);
 
int DeQueue(LinkQueue &LQ, int &e);
```
## 2.3 变量
变量一般采用驼峰命名法，个人也比较喜欢驼峰命名法。

## 2.4 常量、宏定义和枚举
```cpp
#define List_INIT_SIZE 100 
#define LISTINCREMENT 10  
#define TRUE 1
#define FALSE 0
#define OK 1
#define ERROR 0
#define OVERFLOW -1
 
int LENGTH  = 10;
int LIST_MAX_SIZE = 50;
```
# 3. linux下编程风格
Linux 程序的命名习惯和 Windows 程序的命名习惯有很大的不同。一般采用下划线命名法。
```cpp
#define PI 3.141 592 6 
int min_value, max_value;
void send_data(void);
```

>原文链接: https://blog.csdn.net/weixin_42445727/article/details/117235352
