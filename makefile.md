# makefile
##### 基本示例
```
calculator: main.o add.o sub.o mul.o div.o
    gcc main.o add.o sub.o mul.o div.o -o calculator
main.o:main.c
    gcc main.c -o main.o
```
解释
```
{目标}:{依赖}
    {要执行的命令}
```
依赖就是说生成这个目标所需要的文件
##### 自动变量
$@ --> 规则中的目标

$< --> 规则中的第一个依赖条件

$^ --> 规则中的所有依赖条件
```
#示例
app:main.c function1.c function2.c
    gcc $^ -o $@
```
解释:$^则为main.c function1.c function2.c $@则为app