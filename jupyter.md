1. Print something
```python
print ("Hello world")
```
2. Doing math
```python
1 + 1
```

3. More math
```python
1 + 1 / 3
```

4.1 Order of operations matter

```python
(1+1) / 3
```

4.2 Order of operations matter
```python
1 + (1 / 3)
```
5.1 Computers can rember things
```python
x = 1 + 1
```
5.2 Computers can rember things
```python
x
```
6.1 There is a difference between strings and numbers
```python
print ("x")
```

6.2 There is a difference between strings and numbers
```python
print (x)
```

6.3 There is a difference between strings and numbers
```python
# This is not a string. It is a comment
# x = 7
print (x)
# So it didn't change the the variable X
```

7. Computers can do lots of things in a row
```python
x = 10 * 5
print (x)
```
8. And you can combining things together
```python
print ("There are " + str(x) + " states.")
```

9. You can tell computers do things in repeatable chunks.
```python
def adder (x):
    for y in x:
        print (y)
adder ([1, 2])
```

10. computers get mad when you make mistakes
```python
def adder (x):
     for y in x:
          sum = sum + y
     return sum

print (adder ([1, 2]))
```

11. computers get mad when you make mistakes, except when they don't
```python
def adder (x):
     for y in x:
          sum = 0
          sum = sum + y
     return sum
     
print (adder ([1, 2]))
```
11. You need to things right
```python
def adder (x):
     sum = 0
     for y in x:
          sum = sum + y
     return sum
     
print (adder ([1, 2]))
```

12. They get mad about the smallest mistake
```python
print ("Hello world”)
# Do you see the problem?
# Hint: It is a typographical error.
```

13.1 You have to intentionally borrow other peoples code
```python
# Won't work
math.sqrt(2)
```

13.2 You have to intentionally borrow other peoples code
```python
# This will work
import math
math.sqrt(2)
```

13.2 But you can keep borrowing it 
```python
# This will work
math.sqrt(9)
```

14. You can do some really complicated stuff by borrowing other peoples code
```python
import http.client
conn = http.client.HTTPConnection('google.com')
conn.request("GET", "/")
r1 = conn.getresponse()
print(r1.status, r1.reason)
data = r1.read()
print (data)
conn.close()
```


### Installing Jupyter
```shell
ssh  -i "./Documents/TeachPrivacy/AWS/marc_teachprivacy-key-pair-us-east.pem" ubuntu@ec2-54-242-55-200.compute-1.amazonaws.com
sudo apt-get update
sudo apt-get dist-upgrade
sudo reboot
sudo apt-get install python3-pip
sudo -H pip3 install jupyter
jupyter notebook --no-browser --ip 0.0.0.0 --port 8888
```
