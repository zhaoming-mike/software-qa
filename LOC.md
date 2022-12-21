LOC
===

# 代码行数

> 源代码行数简称SLOC，是最简单的一种软件度量，以下以包括注释的实体源代码行数（LOC）为准，说明软件度量的特性及一些限制。
> 以下的C代码只有一行，其LOC为1：

```c
for (i = 0; i < 10; i += 1) printf("hello"); /* How many lines of code is this? */
```

> 但代码在重新排版为以下的代码时，其LOC就从1改变为5，但实际的程序机能没有改变：

```c
/* Now how many lines of code is this? */
for (i = 0; i < 10; i += 1)
{
    printf("hello");
}
```
> 若不使用循环的架构，直接调用10次printf，一般不建议以这种方式撰写程序，但其LOC为11，比上述二个程序的LOC都大：

```c
/* It is not a good code style */
printf("hello");
printf("hello");
printf("hello");
printf("hello");
printf("hello");
printf("hello");
printf("hello");
printf("hello");
printf("hello");
printf("hello");
```

> 不同的软件度量可量测的软件性质也随之不同，像源代码行数适合量测软件的大小，但无法量测软件的模块化程度，而且此度量方式是要量测原代码的长度，不适合作为软件规划阶段进行度量。
