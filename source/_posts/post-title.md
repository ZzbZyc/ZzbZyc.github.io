---
title: post title
date: 2022-02-24 20:38:07
tags:
---

# #汉诺塔

```c
void move(char a,char b) {
    printf("%c ----> %c\n",a,b);
}

void hanno(int n, char a, char b, char c) {
    if(n == 1) {
        move(a,c);
    } else {
        hanno(n-1,a,c,b);
        move(a,c);
        hanno(n-1,b,a,c);
    }
}

int main()
{
    int n;
    scanf("%d",&n);
    hanno(n,'A','B','C');
    return 0;
}
```

