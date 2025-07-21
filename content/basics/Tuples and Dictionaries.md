---
title: Tuples And Dictionaries
date: 2025-07-21
author: Your Name
cell_count: 112
score: 110
---

```python
data = [
    {"name": "Alice", "age": 25},
    {"name": "Bob", "age": 30},
    {"name": "Charlie", "age": 22}
]
print(data)

```

    [{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 22}]
    


```python
employees = [
    {"emp_id": "E01", "name": "Alice", "dept": "HR"},
    {"emp_id": "E02", "name": "Bob", "dept": "IT"},
    {"emp_id": "E03", "name": "Carol", "dept": "Finance"}
]
import json
print(json.dumps(employees, indent=2))

```

    [
      {
        "emp_id": "E01",
        "name": "Alice",
        "dept": "HR"
      },
      {
        "emp_id": "E02",
        "name": "Bob",
        "dept": "IT"
      },
      {
        "emp_id": "E03",
        "name": "Carol",
        "dept": "Finance"
      }
    ]
    


```python
products = [
    {"product": "Laptop", "price": 50000, "in_stock": True},
    {"product": "Mouse", "price": 700, "in_stock": False},
    {"product": "Keyboard", "price": 1200, "in_stock": True}
]
for p in products:
    print(f"{p['product']} - ₹{p['price']} - {'Available' if p['in_stock'] else 'Out of stock'}")

```

    Laptop - ₹50000 - Available
    Mouse - ₹700 - Out of stock
    Keyboard - ₹1200 - Available
    


```python
people = [
    {"name": "Sita", "contact": {"email": "sita@example.com", "phone": "9876543210"}},
    {"name": "Geeta", "contact": {"email": "geeta@example.com", "phone": "8765432109"}}
]
print(json.dumps(people, indent=2))


```

    [
      {
        "name": "Sita",
        "contact": {
          "email": "sita@example.com",
          "phone": "9876543210"
        }
      },
      {
        "name": "Geeta",
        "contact": {
          "email": "geeta@example.com",
          "phone": "8765432109"
        }
      }
    ]
    


```python
library = [
    {"title": "The Alchemist", "author": "Paulo Coelho", "year": 1988},
    {"title": "To Kill a Mockingbird", "author": "Harper Lee", "year": 1960},
    {"title": "1984", "author": "George Orwell", "year": 1949}
]
import pandas as pd
pd.DataFrame(library)

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>title</th>
      <th>author</th>
      <th>year</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>The Alchemist</td>
      <td>Paulo Coelho</td>
      <td>1988</td>
    </tr>
    <tr>
      <th>1</th>
      <td>To Kill a Mockingbird</td>
      <td>Harper Lee</td>
      <td>1960</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1984</td>
      <td>George Orwell</td>
      <td>1949</td>
    </tr>
  </tbody>
</table>
</div>




```python
weather_data = [
    {"date": "2025-07-21", "temp": 34, "humidity": 60},
    {"date": "2025-07-20", "temp": 33, "humidity": 65},
    {"date": "2025-07-19", "temp": 32, "humidity": 70}
]
for entry in weather_data:
    print(f"{entry['date']} → Temp: {entry['temp']}°C, Humidity: {entry['humidity']}%")

```

    2025-07-21 → Temp: 34°C, Humidity: 60%
    2025-07-20 → Temp: 33°C, Humidity: 65%
    2025-07-19 → Temp: 32°C, Humidity: 70%
    


```python
movies = [
    {"movie": "Inception", "rating": 8.8, "year": 2010},
    {"movie": "Interstellar", "rating": 8.6, "year": 2014},
    {"movie": "The Dark Knight", "rating": 9.0, "year": 2008}
]
import json
print(json.dumps(movies, indent=4))

```

    [
        {
            "movie": "Inception",
            "rating": 8.8,
            "year": 2010
        },
        {
            "movie": "Interstellar",
            "rating": 8.6,
            "year": 2014
        },
        {
            "movie": "The Dark Knight",
            "rating": 9.0,
            "year": 2008
        }
    ]
    


```python
results = [
    {"roll_no": 1, "name": "Ajay", "math": 89, "science": 92},
    {"roll_no": 2, "name": "Neha", "math": 95, "science": 96},
    {"roll_no": 3, "name": "Rohit", "math": 78, "science": 85}
]
pd.DataFrame(results)

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>roll_no</th>
      <th>name</th>
      <th>math</th>
      <th>science</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>Ajay</td>
      <td>89</td>
      <td>92</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>Neha</td>
      <td>95</td>
      <td>96</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>Rohit</td>
      <td>78</td>
      <td>85</td>
    </tr>
  </tbody>
</table>
</div>




```python
accounts = [
    {"account_no": "123456", "name": "Kumar", "balance": 20000},
    {"account_no": "654321", "name": "Radha", "balance": 55000},
    {"account_no": "789012", "name": "Divya", "balance": 15000}
]
for acc in accounts:
    print(f"{acc['name']} has ₹{acc['balance']} in account {acc['account_no']}")

```

    Kumar has ₹20000 in account 123456
    Radha has ₹55000 in account 654321
    Divya has ₹15000 in account 789012
    


```python
arr = list(range(20))
print(arr)
```

    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19]
    


```python
arr = list(range(16))
print(arr)
```

    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
    


```python
arr = list(range(30))
print(arr)
```

    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29]
    


```python
arr = list(range(46))
print(arr)
```

    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45]
    


```python
arr = list(range(55))
print(arr)
```

    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54]
    


```python
arr = [x**2 for x in range(17)]
print(arr)
```

    [0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 169, 196, 225, 256]
    


```python
arr = [x**2 for x in range(10)]
print(arr)
```

    [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
    


```python
arr = [x**2 for x in range(500)]
print(arr)
```

    [0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 169, 196, 225, 256, 289, 324, 361, 400, 441, 484, 529, 576, 625, 676, 729, 784, 841, 900, 961, 1024, 1089, 1156, 1225, 1296, 1369, 1444, 1521, 1600, 1681, 1764, 1849, 1936, 2025, 2116, 2209, 2304, 2401, 2500, 2601, 2704, 2809, 2916, 3025, 3136, 3249, 3364, 3481, 3600, 3721, 3844, 3969, 4096, 4225, 4356, 4489, 4624, 4761, 4900, 5041, 5184, 5329, 5476, 5625, 5776, 5929, 6084, 6241, 6400, 6561, 6724, 6889, 7056, 7225, 7396, 7569, 7744, 7921, 8100, 8281, 8464, 8649, 8836, 9025, 9216, 9409, 9604, 9801, 10000, 10201, 10404, 10609, 10816, 11025, 11236, 11449, 11664, 11881, 12100, 12321, 12544, 12769, 12996, 13225, 13456, 13689, 13924, 14161, 14400, 14641, 14884, 15129, 15376, 15625, 15876, 16129, 16384, 16641, 16900, 17161, 17424, 17689, 17956, 18225, 18496, 18769, 19044, 19321, 19600, 19881, 20164, 20449, 20736, 21025, 21316, 21609, 21904, 22201, 22500, 22801, 23104, 23409, 23716, 24025, 24336, 24649, 24964, 25281, 25600, 25921, 26244, 26569, 26896, 27225, 27556, 27889, 28224, 28561, 28900, 29241, 29584, 29929, 30276, 30625, 30976, 31329, 31684, 32041, 32400, 32761, 33124, 33489, 33856, 34225, 34596, 34969, 35344, 35721, 36100, 36481, 36864, 37249, 37636, 38025, 38416, 38809, 39204, 39601, 40000, 40401, 40804, 41209, 41616, 42025, 42436, 42849, 43264, 43681, 44100, 44521, 44944, 45369, 45796, 46225, 46656, 47089, 47524, 47961, 48400, 48841, 49284, 49729, 50176, 50625, 51076, 51529, 51984, 52441, 52900, 53361, 53824, 54289, 54756, 55225, 55696, 56169, 56644, 57121, 57600, 58081, 58564, 59049, 59536, 60025, 60516, 61009, 61504, 62001, 62500, 63001, 63504, 64009, 64516, 65025, 65536, 66049, 66564, 67081, 67600, 68121, 68644, 69169, 69696, 70225, 70756, 71289, 71824, 72361, 72900, 73441, 73984, 74529, 75076, 75625, 76176, 76729, 77284, 77841, 78400, 78961, 79524, 80089, 80656, 81225, 81796, 82369, 82944, 83521, 84100, 84681, 85264, 85849, 86436, 87025, 87616, 88209, 88804, 89401, 90000, 90601, 91204, 91809, 92416, 93025, 93636, 94249, 94864, 95481, 96100, 96721, 97344, 97969, 98596, 99225, 99856, 100489, 101124, 101761, 102400, 103041, 103684, 104329, 104976, 105625, 106276, 106929, 107584, 108241, 108900, 109561, 110224, 110889, 111556, 112225, 112896, 113569, 114244, 114921, 115600, 116281, 116964, 117649, 118336, 119025, 119716, 120409, 121104, 121801, 122500, 123201, 123904, 124609, 125316, 126025, 126736, 127449, 128164, 128881, 129600, 130321, 131044, 131769, 132496, 133225, 133956, 134689, 135424, 136161, 136900, 137641, 138384, 139129, 139876, 140625, 141376, 142129, 142884, 143641, 144400, 145161, 145924, 146689, 147456, 148225, 148996, 149769, 150544, 151321, 152100, 152881, 153664, 154449, 155236, 156025, 156816, 157609, 158404, 159201, 160000, 160801, 161604, 162409, 163216, 164025, 164836, 165649, 166464, 167281, 168100, 168921, 169744, 170569, 171396, 172225, 173056, 173889, 174724, 175561, 176400, 177241, 178084, 178929, 179776, 180625, 181476, 182329, 183184, 184041, 184900, 185761, 186624, 187489, 188356, 189225, 190096, 190969, 191844, 192721, 193600, 194481, 195364, 196249, 197136, 198025, 198916, 199809, 200704, 201601, 202500, 203401, 204304, 205209, 206116, 207025, 207936, 208849, 209764, 210681, 211600, 212521, 213444, 214369, 215296, 216225, 217156, 218089, 219024, 219961, 220900, 221841, 222784, 223729, 224676, 225625, 226576, 227529, 228484, 229441, 230400, 231361, 232324, 233289, 234256, 235225, 236196, 237169, 238144, 239121, 240100, 241081, 242064, 243049, 244036, 245025, 246016, 247009, 248004, 249001]
    


```python
arr = [x**2 for x in range(50)]
print(arr)
```

    [0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 169, 196, 225, 256, 289, 324, 361, 400, 441, 484, 529, 576, 625, 676, 729, 784, 841, 900, 961, 1024, 1089, 1156, 1225, 1296, 1369, 1444, 1521, 1600, 1681, 1764, 1849, 1936, 2025, 2116, 2209, 2304, 2401]
    


```python

arr = [x for x in range(21) if x % 2 == 0]
print(arr)
```

    [0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
    


```python

arr = [x for x in range(22) if x % 2 == 0]
print(arr)
```

    [0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
    


```python

arr = [x for x in range(24) if x % 2 == 0]
print(arr)
```

    [0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22]
    


```python

arr = [x for x in range(50) if x % 2 == 0]
print(arr)
```

    [0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48]
    


```python

arr = [x for x in range(60) if x % 2 == 0]
print(arr)
```

    [0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58]
    


```python
arr = ['a', 'b', 'c', 'd']
print(arr[0])
print(arr[-1])
```

    a
    d
    


```python
arr = ['a', 'b', 'c', 'd']
print(arr[0])
print(arr[-1])
```

    a
    d
    


```python
arr = [1, 2, 3, 4, 5]
arr.append(6)
print(arr)
```

    [1, 2, 3, 4, 5, 6]
    


```python
arr = [10, 20, 30, 40]
arr.pop()
print(arr)
```

    [10, 20, 30]
    


```python
arr = [10, 20, 30, 40,50]
arr.pop()
print(arr)
```

    [10, 20, 30, 40]
    


```python
arr = [10, 20, 30, 40 ,50]
arr.pop()
print(arr)
```

    [10, 20, 30, 40]
    


```python
arr = [10, 20, 30, 40]
arr.pop()
print(arr)
```

    [10, 20, 30]
    


```python
arr = [10, 20, 30, 40]
arr.pop()
print(arr)
```

    [10, 20, 30]
    


```python
arr = [10, 20, 30, 40]
arr.pop()
print(arr)
```

    [10, 20, 30]
    


```python
arr = [10, 20, 30, 40]
arr.pop()
print(arr)
```

    [10, 20, 30]
    


```python
arr = [10, 20, 30, 40]
arr.pop()
print(arr)
```

    [10, 20, 30]
    


```python
arr = [1, 2, 3]
arr.insert(1, 100)
print(arr)
```

    [1, 100, 2, 3]
    


```python
arr = [1, 2, 3,4]
arr.insert(1, 100)
print(arr)
```

    [1, 100, 2, 3, 4]
    


```python
arr = [1, 2, 3]
arr.insert(1, 50)
print(arr)
```

    [1, 50, 2, 3]
    


```python
arr = [1, 2, 3]
arr.insert(1, 200)
print(arr)
```

    [1, 200, 2, 3]
    


```python
arr = [1, 2, 3]
arr.insert(1, 500)
print(arr)
```

    [1, 500, 2, 3]
    


```python
arr = [1, 2, 3]
arr.insert(1, 10)
print(arr)
```

    [1, 10, 2, 3]
    


```python
arr = [1, 2, 3, 4, 5]
print(arr[1:4])
```

    [2, 3, 4]
    


```python
arr = [1, 2, 3, 4, 5]
print(arr[1:5])
```

    [2, 3, 4, 5]
    


```python
arr = [1, 2, 3, 4, 5]
print(arr[1:10])
```

    [2, 3, 4, 5]
    


```python
arr = [1, 2, 3, 4, 5]
print(arr[1:3])
```

    [2, 3]
    


```python
arr = [1, 2, 3, 4, 5]
print(arr[1:2])
```

    [2]
    


```python
arr = [1, 2, 3, 4, 5,6,7]
print(arr[1:4])
```

    [2, 3, 4]
    


```python
arr = [1, 2, 3, 4, 5]
print(arr[1:5])
```

    [2, 3, 4, 5]
    


```python
arr = [1, 2, 3, 4, 5,6,7,8,9,10]
print(arr[1:4])
```

    [2, 3, 4]
    


```python
# Cell 86 - Python Arrays
arr = [1, [2, 3], [4, 5]]
print(arr[1][1])
```

    3
    


```python
arr = [1, [2, 3], [4, 5]]
print(arr[1][1])
```

    3
    


```python
arr = [x for x in range(10)]
print(sum(arr))
```

    45
    


```python
d = {str(x): x**2 for x in range(3)}
print(d)
```

    {'0': 0, '1': 1, '2': 4}
    


```python
d = {str(x): x**2 for x in range(4)}
print(d)
```

    {'0': 0, '1': 1, '2': 4, '3': 9}
    


```python
d = {str(x): x**2 for x in range(7)}
print(d)
```

    {'0': 0, '1': 1, '2': 4, '3': 9, '4': 16, '5': 25, '6': 36}
    


```python
d = {str(x): x**2 for x in range(9)}
print(d)
```

    {'0': 0, '1': 1, '2': 4, '3': 9, '4': 16, '5': 25, '6': 36, '7': 49, '8': 64}
    


```python
d = {'name': 'Alice', 'age': 25}
print(d['name'])
```

    Alice
    


```python
d = {'name': 'Alice', 'age': 25}
print(d['age'])
```

    25
    


```python
d = {'name': 'Alice', 'age': 25}
print(d['name'])
```

    Alice
    


```python
d = {'name': 'Alice', 'age': 25}
print(d['name'])
```

    Alice
    


```python
d = {'a': 1, 'b': 2}
d['c'] = 3
print(d)
```

    {'a': 1, 'b': 2, 'c': 3}
    


```python
d = {'a': 1, 'b': 2}
d['c'] = 3
print(d)
```

    {'a': 1, 'b': 2, 'c': 3}
    


```python

d = {'a': 1, 'b': 2}
d['c'] = 3
print(d)



```

    {'a': 1, 'b': 2, 'c': 3}
    


```python
d = {'a': 1, 'b': 2}
d['c'] = 3
print(d)
```

    {'a': 1, 'b': 2, 'c': 3}
    


```python
d = {'x': 10, 'y': 20}
print(list(d.keys()))
```

    ['x', 'y']
    


```python
d = {'x': 10, 'y': 20}
print(list(d.keys()))
```

    ['x', 'y']
    


```python
d = {'x': 10, 'y': 20}
print(list(d.items()))
```

    [('x', 10), ('y', 20)]
    


```python
d = {'x': 10, 'y': 20}
print(list(d.items()))
```

    [('x', 10), ('y', 20)]
    


```python
d = {'x': 10, 'y': 20}
print(list(d.items()))
```

    [('x', 10), ('y', 20)]
    


```python
d1 = {'a': 1}
d2 = {'b': 2}
d1.update(d2)
print(d1)
```

    {'a': 1, 'b': 2}
    


```python
students = [
    ("Ravi", 90),
    ("Priya", 85),
    ("Aman", 78)
]

for name, marks in students:
    print(f"{name} scored {marks}")

```

    Ravi scored 90
    Priya scored 85
    Aman scored 78
    


```python
student = {
    "name": "Kiran",
    "dob": (2002, 5, 23),  # (year, month, day)
    "marks": (89, 92, 85)
}
print(student["dob"])

```

    (2002, 5, 23)
    


```python
coordinates = [
    (0, 0),
    (1, 2),
    (3, 4),
    (5, 6)
]

for x, y in coordinates:
    print(f"x={x}, y={y}")

```

    x=0, y=0
    x=1, y=2
    x=3, y=4
    x=5, y=6
    


```python
colors = ["red", "green", "blue"]

for index, color in enumerate(colors):
    print(f"Index: {index}, Color: {color}")

```

    Index: 0, Color: red
    Index: 1, Color: green
    Index: 2, Color: blue
    


```python
def min_max(numbers):
    return (min(numbers), max(numbers))

result = min_max([10, 5, 2, 99])
print(f"Min: {result[0]}, Max: {result[1]}")

```

    Min: 2, Max: 99
    


```python
person_info = (
    ("Name", "Ravi"),
    ("Age", 24),
    ("Gender", "Male")
)

for label, value in person_info:
    print(f"{label}: {value}")

```

    Name: Ravi
    Age: 24
    Gender: Male
    


```python
employee = ("Raj", "Developer", 50000)

name, role, salary = employee
print(f"{name} works as a {role} earning ₹{salary}")

```

    Raj works as a Developer earning ₹50000
    


```python
students = [
    ("Ravi", 90),
    ("Priya", 85),
    ("Aman", 78)
]

# Sort by marks
sorted_students = sorted(students, key=lambda x: x[1], reverse=True)
print(sorted_students)

```

    [('Ravi', 90), ('Priya', 85), ('Aman', 78)]
    


```python
location_map = {
    (12.9716, 77.5946): "Bangalore",
    (28.6139, 77.2090): "Delhi"
}
print(location_map[(12.9716, 77.5946)])


```

    Bangalore
    


```python
contacts = (
    ("Ravi", ("ravi@example.com", "9876543210")),
    ("Priya", ("priya@example.com", "8765432109"))
)

for name, (email, phone) in contacts:
    print(f"{name} → Email: {email}, Phone: {phone}")

```

    Ravi → Email: ravi@example.com, Phone: 9876543210
    Priya → Email: priya@example.com, Phone: 8765432109
    


```python
names = ["Amit", "Sita", "John"]
scores = [88, 92, 79]

zipped = list(zip(names, scores))
print(zipped)  # [('Amit', 88), ('Sita', 92), ('John', 79)]

```

    [('Amit', 88), ('Sita', 92), ('John', 79)]
    


```python
my_list = [1, 2, 3]
my_tuple = tuple(my_list)
print(my_tuple)  # (1, 2, 3)

back_to_list = list(my_tuple)
print(back_to_list)  # [1, 2, 3]

```

    (1, 2, 3)
    [1, 2, 3]
    


```python
def get_student():
    return ("Kavya", 20, "BSc")

name, age, course = get_student()
print(f"{name} is {age} years old and studies {course}")

```

    Kavya is 20 years old and studies BSc
    


```python
a = 5
b = 10

a, b = b, a  # Swap
print(f"a = {a}, b = {b}")

```

    a = 10, b = 5
    


```python
data = (
    {"name": "Ravi", "score": 80},
    {"name": "Anu", "score": 95},
    {"name": "Kiran", "score": 70}
)

for entry in data:
    print(entry["name"], entry["score"])

```

    Ravi 80
    Anu 95
    Kiran 70
    


```python
import pandas as pd

data = [
    ("Kiran", 80, 90),
    ("Ravi", 70, 85),
    ("Anu", 95, 100)
]

df = pd.DataFrame(data, columns=["Name", "Maths", "Science"])
df

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Maths</th>
      <th>Science</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Kiran</td>
      <td>80</td>
      <td>90</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Ravi</td>
      <td>70</td>
      <td>85</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Anu</td>
      <td>95</td>
      <td>100</td>
    </tr>
  </tbody>
</table>
</div>




```python
def sum_all(*numbers):
    return sum(numbers)

print(sum_all(1, 2, 3))     # 6
print(sum_all(10, 20, 30))  # 60

```

    6
    60
    


```python
items = ["apple", "banana", "grape"]

for idx, val in enumerate(items):
    print(f"{idx}: {val}")

```

    0: apple
    1: banana
    2: grape
    


```python
# Use tuple for fixed data (e.g., months)
months = ("Jan", "Feb", "Mar", "Apr")
# months[0] = "January"  ❌ Will throw error
print(months)

```

    ('Jan', 'Feb', 'Mar', 'Apr')
    


```python
rows = [
    (1, "Kiran", "B.Tech"),
    (2, "Sita", "B.Sc"),
    (3, "Ravi", "MCA")
]

for roll, name, course in rows:
    print(f"{roll} - {name} - {course}")

```

    1 - Kiran - B.Tech
    2 - Sita - B.Sc
    3 - Ravi - MCA
    


```python
config = ("localhost", 8080)
host, port = config
print(f"Server running on {host}:{port}")

```

    Server running on localhost:8080
    


```python
marks = [
    ("Ajay", [78, 85, 90]),
    ("Kavya", [88, 92, 95]),
    ("Rohit", [65, 70, 72])
]

for name, scores in marks:
    print(f"{name} → Avg = {sum(scores)/len(scores):.2f}")

```

    Ajay → Avg = 84.33
    Kavya → Avg = 91.67
    Rohit → Avg = 69.00
    


```python
coordinates = {
    (0, 0),
    (1, 2),
    (3, 4)
}

print((1, 2) in coordinates)  # True

```

    True
    


```python
matrix = (
    (1, 2, 3),
    (4, 5, 6),
    (7, 8, 9)
)

for row in matrix:
    print(row)

```

    (1, 2, 3)
    (4, 5, 6)
    (7, 8, 9)
    


```python
scores = [
    ("Alice", 88),
    ("Bob", 75),
    ("Charlie", 95)
]

sorted_scores = sorted(scores, key=lambda x: x[1])
print(sorted_scores)

```

    [('Bob', 75), ('Alice', 88), ('Charlie', 95)]
    


```python
student = {"name": "Meena", "age": 21, "course": "B.Tech"}

for key, value in student.items():
    print(f"{key}: {value}")

```

    name: Meena
    age: 21
    course: B.Tech
    


```python
from itertools import product

colors = ["Red", "Green"]
sizes = ["S", "M"]

combos = list(product(colors, sizes))
print(combos)
# [('Red', 'S'), ('Red', 'M'), ('Green', 'S'), ('Green', 'M')]

```

    [('Red', 'S'), ('Red', 'M'), ('Green', 'S'), ('Green', 'M')]
    


```python
nested = ((1, 2), (3, 4), (5, 6))
flat = [item for sub in nested for item in sub]
print(flat)  # [1, 2, 3, 4, 5, 6]

```

    [1, 2, 3, 4, 5, 6]
    


```python
def show_data(info):
    for item in info:
        print(item)

show_data(("Python", "Tuples", "Immutable"))

```

    Python
    Tuples
    Immutable
    


```python
votes = [
    ("Alice", "Yes"),
    ("Bob", "No"),
    ("Alice", "Yes"),
    ("Alice", "No")
]

from collections import Counter
vote_counter = Counter(votes)
print(vote_counter)

```

    Counter({('Alice', 'Yes'): 2, ('Bob', 'No'): 1, ('Alice', 'No'): 1})
    


```python
from collections import namedtuple

Student = namedtuple("Student", "name age grade")
s1 = Student("Amit", 20, "A")

print(s1.name, s1.age, s1.grade)


```

    Amit 20 A
    


```python
person = ("Ram", 35, "Teacher")
print(f"Name: {person[0]}, Age: {person[1]}, Occupation: {person[2]}")

```

    Name: Ram, Age: 35, Occupation: Teacher
    


```python
names = ("Ravi", "Seema", "Arun")
ages = (25, 30, 22)

for name, age in zip(names, ages):
    print(f"{name} is {age} years old")

```

    Ravi is 25 years old
    Seema is 30 years old
    Arun is 22 years old
    


```python
mixed = ("Python", [1, 2, 3])
mixed[1].append(4)
print(mixed)  # ('Python', [1, 2, 3, 4])

```

    ('Python', [1, 2, 3, 4])
    


```python
a = (1, 2, 3)
b = (1, 2, 4)
print(a < b)  # True (compares element-wise)

```

    True
    


```python
def analyze_data(data):
    average = sum(data) / len(data)
    return (min(data), max(data), average)

result = analyze_data([10, 20, 30, 40])
print(f"Min: {result[0]}, Max: {result[1]}, Avg: {result[2]}")

```

    Min: 10, Max: 40, Avg: 25.0
    


```python
d = {'a': {'x': 10, 'y': 20}, 'b': 2}
print(d['a']['y'])
```

    20
    


```python
d = {'a': {'x': 10, 'y': 20}, 'b': 2}
print(d['a']['x'])
```

    10
    


```python
d = {'apple': 3, 'banana': 2}
print(sum(d.values()))
```

    5
    


```python
d = {'apple': 3, 'banana': 2}
print(sum(d.values()))
```

    5
    


```python
d = {'apple': 3, 'banana': 2}
print(sum(d.values()))
```

    5
    


```python
d1 = {'a': 1}
d2 = {'b': 2}
d1.update(d2)
print(d1)
```

    {'a': 1, 'b': 2}
    


```python

```


---
**Score: 110**