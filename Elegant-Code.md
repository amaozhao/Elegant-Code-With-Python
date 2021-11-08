## 1. 操作符之间留有空格

Hmmm

```python
a= 3+ 5
```

优雅的

```python
a = 3 + 5
```

## 2. 在多行中分配变量
Hmmm

```python
a, b = 3, 5
```

优雅的

```python
a = 3
b = 5
```

## 3. 正确命名变量

Hmmm

```python
a = 3
b = 5
c = a + b
```

优雅的

```python
first_number = 3
second_number = 5
total = first_number + second_number
```

## 4. 缩进 4 个空格而不是 2 个

将键入代码放入块缩进 4 个空格而不是 2 个空格时

Hmmm

```python
i = 0

while i < 10:
  print (i)
  i += 1
```

优雅的

```python
i = 0

while i < 10:
    print (i)
    i += 1
```

## 5. 在逻辑代码组之间留一条线
### 5.1. 示例 1

```python
i = 0
while i < 10:
    print (i)
    i += 1
```

优雅的

```python
i = 0

while i < 10:
    print (i)
    i += 1
```

### 5.2. 示例 2

```python
first_number = 3
second_number = 5
total = first_number + second_number
print ("total is " + str(total))
```

优雅的
留下一行清楚地分隔变量分配、总计和打印结果。

```python
first_number = 3
second_number = 5

total = first_number + second_number

print ("total is " + str(total))
```

## 6. 使用 for 而不是 while

```python
i = 0

while i < 10:
    print (i)
    i += 1
```

优雅的

```python
for i in range(10):
    print (i)
```

## 7. 使用双等号进行比较

The code below won’t work

```python
a = 3

if (a = 5):
    print ("a is equal to 5" )
else :
    print ("a is not equal to 5" )
```

优雅的

```python
a = 3

if (a == 5):
     print ("a is equal to 5" )
else :
    print ("a is not equal to 5" )
```

## 8. 使用列表理解

```python
numbers = [1, 2, 3, 4, 5]

numbers_doubled = []

for number in numbers:
    numbers_doubled.append(number * 2)

print (numbers_doubled)
```

优雅的

```python
numbers = [1, 2, 3, 4, 5]

numbers_doubled = [number * 2 for number in numbers]

print (numbers_doubled)
```

## 9. 函数名应该说明它们的作用

```python
def area(radius):
    return 3.14 * radius * radius

radius = 7

print ("Area of circle: " )
print (area(7))
```

优雅的

```python
def area_of_circle(radius):
    return 3.14 * radius * radius

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

## 10. 提取常量到代码顶部

```python
def area_of_circle(radius):
    return 3.14 * radius * radius

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

优雅的

```python
PI = 3.14

def area_of_circle(radius):
    return PI * radius * radius

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

## 11. 给出正确的参数名称

```python
PI = 3.14

def area_of_circle(r):
    return PI * r * r

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

优雅的

```python
PI = 3.14

def area_of_circle(radius):
    return PI * radius * radius

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

## 12. 常量应该全部大写

```python
Pi = 3.14

def area_of_circle(radius):
    return Pi * radius * radius

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

优雅的

```python
PI = 3.14

def area_of_circle(radius):
    return PI * radius * radius

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

## 13. 使用 Python 提供的数学常量
```python
PI = 3.14

def area_of_circle(r):
    return PI * r * r

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

优雅的

```python
import math 

def area_of_circle(r):
    return math.pi * r * r

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

## 14. 不要将 Lambda 分配给变量
```python
import math 

area_of_circle = lambda radius: math.pi * radius * radius

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

优雅的

```python
import math 

def area_of_circle(radius):
    return math.pi * radius * radius

radius = 7

print ("Area of circle: " )
print (area_of_circle(7))
```

## 15. 提取通用代码到 Lambda
```python
double = lambda number: number * 2
triple = lambda number: number * 3

print (double(2))
print (triple(2))
```

优雅的

```python
def multiplier(multiplier):
    return lambda number : number * multiplier

double = multiplier(2)
triple = multiplier(3)

print (double(2))
print (triple(2))
```

## 16.类名应该以大写字母开头
```python
class foo :
    def __init__(self):
        print ("foo initialized" )

foo_instance = foo()
```

优雅的

```python
class Foo :
    def __init__(self):
        print ("foo initialized" )

foo_instance = Foo()
```

## 17. 不要从模块中导入所有内容
```python
from some_module import * 

print_something()
```

优雅的

```python
from some_module import print_something

print_something()
```

## 18. 变量名不应包含大写字母
```python
FirstNumber = 3
SecondNumber = 5

Total = FirstNumber + SecondNumber
```

优雅的

```python
first_number = 3
second_number = 5

total = first_number + second_number
```

## 19. 在变量中用下划线分隔单词
```python
firstnumber = 3
secondnumber = 5
```

优雅的

```python
first_number = 3
second_number = 5
```

## 20. 使用下划线使大数可读
```python
large_number = 3458634
```

优雅的

```python
large_number = 3_458_634
```

## 21. 函数名不应该是驼峰式或蛇式

### 21.1. 避免驼峰式函数

```python
def FooBar():
  # Do something
```

优雅的

```python
def foo_bar():
  # Do something
```

### 21.2. 避免 Snake Case 函数

```python
def fooBar():
  # Do something
```

优雅的

```python
def foo_bar():
  # Do something
```

## 22.类名应该是驼峰式的

### 22.1. 示例 1

```python
class square ():
  # Do something
```

优雅的

```python
class Square ():
  # Do something
```
### 22.2. 示例 2

```python
class fooBar ():
  # Do something
```

优雅的

```python
class FooBar ():
  # Do something
```
### 22.3. 示例 3

```python
class foo_bar ():
  # Do something
```

优雅的

```python
class FooBar ():
  # Do something
```

## 23. 有合理的类名

在这里，我使用一个名为 FooBar 的类来向您解释 Python 中的类。

```python
class FooBar ():
  # Do something
```

优雅的
我可以改用一个名为 SampleClass 的名称，它可以更好地描述它的用途。

```python
class SampleClass ():
  # Do something
```

## 24.避免链等于
```python
a = b = c = 5
```

优雅的

```python
a = 5
b = 5
c = 5
```

## 25. 如果可能，继承类并重用代码
```python
class Rectangle ():
    def __init__(self, length, breadth):
        self.length = length
        self.breadth = breadth

    def area(self):
        return self.length * self.breadth

class Square ():
    def __init__(self, side_length):
        self.side_length = side_length

    def area(self):
        return self.side_length * self.side_length

square = Square(5)
print (square.area())
```

优雅的

```python
class Rectangle ():
    def __init__(self, length, breadth):
        self.length = length
        self.breadth = breadth

    def area(self):
        return self.length * self.breadth

class Square (Rectangle):
    def __init__(self, side_length):
         self.length = side_length
        self.breadth = side_length

square = Square(5)
print (square.area())
```

请注意我们如何通过继承 Rectangle 避免为 Square 编写函数 area() 。

## 26. 如果实例变量反映类名更好

```python
class Circle ():
    def __init__(self, radius):
        self.radius = radius

c = Circle(7)
```

优雅的

```python
class Circle ():
    def __init__(self, radius):
        self.radius = radius

circle = Circle(7)
```

## 27. 内部常量应该以下划线开头
```python
class Circle ():
    PI = 22 / 7

    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return self.PI * self.radius * self.radius


circle = Circle(7)
print (circle.area())
```

优雅的

```python
class Circle ():
    _PI = 22 / 7

    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return self._PI * self.radius * self.radius


circle = Circle(7)
print (circle.area())
```

## 28. 存储经常计算的值
```python
first_number = 3
second_number = 5

print (f " { first_number} X { second_number} = { first_number * second_number} " )
print (f " { second_number} X { first_number} = { first_number * second_number} " )
```

优雅的

```python
first_number = 3
second_number = 5

product = first_number * second_number

print (f " { first_number} X { second_number} = { product} " )
print (f " { second_number} X { first_number} = { product} " )
```

## 29. 使用 f 字符串
```python
first_number = 3
second_number = 5

product = first_number * second_number

print (str(first_number) + " X " + str(second_number) + " = " + str(product))
```

优雅的

```python
first_number = 3
second_number = 5

product = first_number * second_number

print (f " { first_number} X { second_number} = { product} " )
```

## 30. 避免在一行中使用多个语句
```python
print ('foo' ); print ('bar' )
```

优雅的

```python
print ('foo' )
print ('bar' )
```

## 31. 避免单行 if 语句
```python
x = 1

if x == 1: print ("One" )
```

优雅的

```python
x = 1

if x == 1:
    print ("One" )
```

## 32. 在 If 语句之前评估复杂条件
```python
a = 10
b = 6
c = 7

if a > b and a > c:
    print ("a is greatest" )
```

优雅的
虽然更冗长，但以下代码更具可读性。

```python
a = 10
b = 6
c = 7

a_greater_than_b = a > b
a_greater_than_c = a > c
a_is_the_greatest = a_greater_than_b and a_greater_than_c

if a_is_the_greatest:
    print ("a is greatest" )
```

## 33. 使参数传递更加明确
```python
def add_two_numbers(* numbers):
    first_number, second_number = numbers
    return first_number + second_number

total = add_two_numbers(3, 5)
print (total)
```

优雅的

```python
def add_two_numbers(first_number, second_number):
    return first_number + second_number

total = add_two_numbers(3, 5)
print (total)
```

## 34. 让你的代码读起来像文档一样
```python
def add_two_numbers(first_number, second_number):
    return first_number + second_number

total = add_two_numbers(3, 5)
print (total)
```

优雅的

```python
def add_two_numbers(first_number, second_number):
    sum_of_two_numbers = first_number + second_number
    return sum_of_two_numbers

total = add_two_numbers(3, 5)
print (total)
```

## 35. 给返回变量的正确名称
```python
def add_two_numbers(first_number, second_number):
    output = first_number + second_number
    return output

total = add_two_numbers(3, 5)
print (total)
```

优雅的

```python
def add_two_numbers(first_number, second_number):
    sum_of_two_numbers = first_number + second_number
    return sum_of_two_numbers

total = add_two_numbers(3, 5)
print (total)
```

## 36. 对一次性变量使用下划线
```python
people = [
    ('Karthikeyan' , 'Tech Guy' ),
    ('Shakes Sphere' , 'Author' ),
    ('Thiru Valluvar' , 'Philosopher' ),
    ('Jesus' , 'Son of God' ),
    ('Nithyanadha' , 'God' )
]


# We print only names of people
for name, profession in people:
    print (name)
```

优雅的

```python
people = [
    ('Karthikeyan' , 'Tech Guy' ),
    ('Shakes Sphere' , 'Author' ),
    ('Thiru Valluvar' , 'Philosopher' ),
    ('Jesus' , 'Son of God' ),
    ('Nithyanadha' , 'God' )
]


# We print only names of people
# so we use throw away varible for
# profession
for name, _ in people:
    print (name)
```

## 37. 如果列表不可变，则使用元组
```python
pythogorean_triplet = [3, 4, 5]
```

优雅的

```python
pythogorean_triplet = (3, 4, 5)
```

## 38. 使用 With 打开文件进行阅读
```python
file = open('file.txt' )
file_content = file.read()
print (file_content)
file.close()
```

优雅的

```python
with open('file.txt' ) as file:
    file_content = file.read()
    print (file_content)
```

## 39. 为文件句柄使用合理的名称
```python
f = open('file.txt' )
file_content = f.read()
print (file_content)
f.close()
```

优雅的
尽管名称 f 用于处理文件对象，但请使用适当的名称，例如 file ，或者最好使用与您打开的文件相关的名称，以便代码更易于理解。

```python
file = open('file.txt' )
file_content = file.read()
print (file_content)
file.close()
```

## 40. 使用过滤器
```python
numbers = [1, 5, 12, 6, 4, 7, 18, 21]
odd_numbers = []

for number in numbers:
    if number % 2 != 0:
        odd_numbers.append(number)

print (odd_numbers)
```

优雅的
使用过滤器意味着您可以将复杂的过滤逻辑抽象为过滤器功能。

```python
def filter_odd_numbers(number):
    return True if (number % 2 != 0) else False

numbers = [1, 5, 12, 6, 4, 7, 18, 21]
odd_numbers_filter = filter(filter_odd_numbers, numbers)

print ([odd_number for odd_number in odd_numbers_filter])
```

## 41. 使用列表理解过滤
```python
numbers = [1, 5, 12, 6, 4, 7, 18, 21]
odd_numbers = []

for number in numbers:
    if number % 2 != 0:
        odd_numbers.append(number)

print (odd_numbers)
```

优雅的
当您需要进行非常简单的过滤操作时，列表理解中的一个简单条件就足够了。

```python
numbers = [1, 5, 12, 6, 4, 7, 18, 21]
odd_numbers = [number for number in numbers if number % 2 != 0]
print (odd_numbers)
```

## 42. 使用双等于而不是 is
### 42.1. 示例 1
```python
number = 42

if number is 42:
    print ("Found the answer to ultimate question!" )
```

优雅的

```python
number = 42

if number == 42:
    print ("Found the answer to ultimate question!" )
```
### 42.2. 示例 2
```python
a = 42
b = 42.0

print (a is b)
```

优雅的

```python
a = 42
b = 42.0

print (a == b)
```

## 43. 合并字典
```python
dict_1 = { 'a': 1, 'b': 2 }
dict_2 = { 'c': 3, 'd': 4 }

merged_dict = {}

for key in dict_1:
    merged_dict[key] = dict_1[key]

for key in dict_2:
    merged_dict[key] = dict_2[key]

print (merged_dict)
```
优雅的
```python
dict_1 = { 'a': 1, 'b': 2 }
dict_2 = { 'c': 3, 'd': 4 }

merged_dict = { ** dict_1, ** dict_2 }
print (merged_dict)
```
## 44. 在花括号周围留出空间
```python
person = {'name': 'Karthik' }
```
优雅的
```python
person = { 'name': 'Karthik' }
```
## 45. 不要在字典中的键和冒号之间留空格
```python
{ 'name' : 'Karthik' }
```
优雅的
```python
{ 'name': 'Karthik' }
```
## 46. 在字典中在冒号和值之间留出空格
```python
person = { 'name':'Karthik' }
```
优雅的
```python
person = { 'name': 'Karthik' }
```
## 47. 如果字典太大，则使字典多行
```python
phone_numbers = { 'Karthik' : '12345' , 'Ashok' : '67890' , 'Babu' : '4321' , 'Ganesh' : '83782' }
```
优雅的
```python
phone_numbers = {
    'Karthik': '12345' ,
    'Ashok': '67890' ,
    'Babu': '4321' ,
    'Ganesh': '83782' 
}
```

## 48. 使用类型注解
```python
def add_two_numbers(first_number, second_number):
    return first_number + second_number
```
优雅的
类型注释有助于静态代码检查和更好的帮助文档。
```python
def add_two_numbers(first_number: int, second_number: int) -> int:
    return first_number + second_number
```
## 49. 在 Python REPL 中测试小代码片段
```python
$ python
Python 3.8.5 (default, Sep  4 2020, 02:22:02)
[Clang 10.0.0 ] :: Anaconda, Inc. on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import math
>>> def circle_area(radius): return math.pi * radius ** 2
...
>>> circle_area(7)
153.93804002589985
>>>
```
## 50. 在 REPL 中使用下划线访问最后计算的值
```python
>>> 1 + 2
3
>>> _ * 3
9
```
## 51. 退出 REPL
```python
$ python
Python 3.8.5 (default, Sep  4 2020, 02:22:02)
[Clang 10.0.0 ] :: Anaconda, Inc. on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import math
>>> def circle_area(radius): return math.pi * radius ** 2
...
>>> circle_area(7)
153.93804002589985
>>> height = 10
>>> _
153.93804002589985
>>> _ * height
1539.3804002589986
>>>
>>>
>>> 1 + 2
3
>>> _ * 3
9
>>> exit()
```
通过键入 Ctrl + D 或 exit() 退出 REPL。

## 52.禅

```python
$ python
Python 3.8.5 (default, Sep  4 2020, 02:22:02)
[Clang 10.0.0 ] :: Anaconda, Inc. on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import this
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```
