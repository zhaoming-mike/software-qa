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
