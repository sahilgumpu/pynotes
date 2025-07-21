---
title: Strings
date: 2025-07-21
author: Your Name
cell_count: 20
score: 20
---

```python
m= 'HellO World'
```


```python
print(len(m))
```

    11
    


```python
print(s.upper())
```

    HELLO WORLD
    


```python
print(s.lower())
```

    hello world
    


```python
print(s.capitalize())
```

    Hello world
    


```python
print(s.title())
```

    Hello World
    


```python
print(s.find('e'))
      
```

    1
    


```python
print(s.find('r'))
```

    8
    


```python
print(s.find('d'))
```

    10
    


```python
print(s.find('w'))
```

    6
    


```python
print('  test  '.lstrip())
```

    test  
    


```python
print('123'.isdigit())
```

    True
    


```python
print('12345'.isdigit())
```

    True
    


```python
print('one1two2'.translate(str.maketrans('', '', '0123456789')))
```

    onetwo
    


```python
print('abcdefghijklmno'.find('j', 5))
```

    9
    


```python
print('abcdefghijklmno'.find('a', 5))
```

    -1
    


```python
print('abcdefghijklmno'.find('k', 5))
```

    10
    


```python
print('abcdefghijklmno'.find('n', 5))
```

    13
    


```python
print('abc'.__add__('123'))
```

    abc123
    


```python

```


---
**Score: 20**