---
title: "python_code_snippets"
date: 2022-04-11T17:45:10-04:00
draft: false
---

cache decorator - increase speed of math calculations
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

test function
```python
def myfunc(a,b):
    if a>b:
        print ("It worked")
    
    else:
        print ("No")
        
myfunc(2,1)
```

if_else
```python
hungry = True

if hungry:
    print('FEED ME NOW!')
else:
    print("I'M NOT HUNGRY!!!")
```

if_elif_else
```python
loc = 'Store'
if loc == 'Auto Shop':
    print("Cars are cool!!!")
elif loc  == 'Bank':
    print('Money is cool!!!')
elif loc == 'Store':
    print('Welcome to the store!')
else:
    print("I do not know much")
```

if_elif_else
```python
loc = 'Store'
if loc == 'Auto Shop':
    print("Cars are cool!!!")
elif loc  == 'Bank':
    print('Money is cool!!!')
elif loc == 'Store':
    print('Welcome to the store!')
else:
    print("I do not know much")
```

get ip address
```python
import requests

response = requests.get('https://httpbin.org/ip')

print('Your IP is {0}'.format(response.json()['origin']))
```