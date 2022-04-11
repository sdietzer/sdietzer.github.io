---
title: "python_code_snippets"
date: 2022-04-11T17:45:10-04:00
draft: false
---

cache decorator
```python
from functools import cache, lru_cache


@lru_cache(maxsize=5)
def fib(n):
    if n <= 1:
        return n
    return fib(n - 1) + fib(n - 2)


def main():
    for i in range(400):
        print(i, fib(i))
    print("done")


if __name__ == '__main__':
    main()
```