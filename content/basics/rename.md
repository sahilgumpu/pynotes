---
title: Rename
date: 2025-07-21
author: Your Name
cell_count: 55
score: 55
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

```


---
**Score: 55**