```python
%timeit sum(range(100))
```

    545 ns ± 5.26 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
    


```python
%timeit sum(range(1000000))
```

    14.9 ms ± 657 μs per loop (mean ± std. dev. of 7 runs, 100 loops each)
    


```python
%pdb
numbers = "hello"

sum(numbers)
```

    Automatic pdb calling has been turned OFF
    


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[13], line 4
          1 get_ipython().run_line_magic('pdb', '')
          2 numbers = "hello"
          3 
    ----> 4 sum(numbers)
    

    TypeError: unsupported operand type(s) for +: 'int' and 'str'



```python
name = "Jackson"
age = 27
scores = [90, 85, 100, 77]


```


```python
del name
```


```python
%whos
```

    Variable   Type    Data/Info
    ----------------------------
    age        int     27
    numbers    str     hello
    scores     list    n=4
    


```python
%history -n
```

       1: %pdb
       2:
    total = sum("hello")
    print(total)
       3:
    total = sum("hello")
    print(total)
       4: %pdb
       5: %pdb
       6: %pdb
       7:
    numbers = "hello"
    sum(numbers)
       8:
    %pdb
    numbers = "hello"
    sum(numbers)
       9:
    %pdb
    numbers = "hello"
    sum(numbers)
      10:
    %pdb
    numbers = "hello"
    sum(numbers)
      11:
    %pdb
    numbers = "hello"
    sum(numbers)
      12:
    %pdb
    numbers = "hello"
    sum(numbers)
      13:
    %pdb
    numbers = "hello"
    
    sum(numbers)
      14: %whos
      15: %whos
      16:
    name = "Jackson"
    age = 27
    scores = [90, 85, 100]
      17: %whos
      18:
    name = "Jackson"
    age = 27
    scores = [90, 85, 100, 77]
      19: %whos
      20: del name
      21: %whos
      22:
    name = "Jackson"
    age = 27
    scores = [90, 85, 100, 77]
      23: %whos
      24: del name
      25: %whos
      26: %history
      27: %history -n
    


```python
%reset
```


```python
%history
```

    %pdb
    total = sum("hello")
    print(total)
    total = sum("hello")
    print(total)
    %pdb
    %pdb
    %pdb
    numbers = "hello"
    sum(numbers)
    %pdb
    numbers = "hello"
    sum(numbers)
    %pdb
    numbers = "hello"
    sum(numbers)
    %pdb
    numbers = "hello"
    sum(numbers)
    %pdb
    numbers = "hello"
    sum(numbers)
    %pdb
    numbers = "hello"
    sum(numbers)
    %pdb
    numbers = "hello"
    
    sum(numbers)
    %whos
    %whos
    name = "Jackson"
    age = 27
    scores = [90, 85, 100]
    %whos
    name = "Jackson"
    age = 27
    scores = [90, 85, 100, 77]
    %whos
    del name
    %whos
    name = "Jackson"
    age = 27
    scores = [90, 85, 100, 77]
    %whos
    del name
    %whos
    %history
    %history -n
    %reset
    %history
    


```python
%whos
```

    Interactive namespace is empty.
    


```python
%%writefile hello.py
print("Hello from a real Python file")
```

    Writing hello.py
    


```python
%pwd
```




    'c:\\Users\\jacks\\Desktop\\TestTest'




```python
%run hello.py
```

    Hello from a real Python file
    
