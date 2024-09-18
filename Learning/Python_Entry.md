<div style="text-align: center;">
    <h1><u>PYTHON</u></h1>
</div>

<h4><u>EXCEPTIONS</u></h4>

### What is an Exception?

An **exception** in programming is like when something unexpected happens, and the program doesn't know how to continue. Think of it as a little "oops" moment where something goes wrong, like trying to divide by zero or opening a book (file) that doesn't exist. Instead of stopping the program completely, exceptions help us manage these errors by letting us fix or handle the problem.

### How Exceptions Work

Let's imagine you're baking a cake, and you go to grab some flour, but it's all gone—oops! Instead of stopping baking entirely, you can handle the situation by going to the store or using a substitute ingredient.

In programming, if we expect that something might go wrong, we can use **try** and **except** blocks to prepare for it. So, when an error (or exception) happens, the program can "catch" the exception and respond to it instead of crashing.

For example, if you try to open a file that doesn't exist, Python might raise an **Exception**. You can handle this like so:

```python
try:
    open('non_existing_file.txt')
except FileNotFoundError:
    print("Oops! File not found. Let's create a new one.")
```

### Why Exceptions are Useful

By using exceptions, we can make sure our programs keep running smoothly, even when something unexpected happens. Exceptions are like traffic lights for errors—they help guide the program so it doesn't crash and can keep going.

### Python Try Except

- The **try** block lets you test a block of code for errors.
- The **except** block lets you handle the error.
- The **else** block lets you execute code when there is no error.
- The **finally** block lets you execute code, regardless of the result of the try and except blocks.

#### Example:

````python
try:
    number = int(input("Enter a number: "))
    result = 10 / number
except ZeroDivisionError:
    print("Oops! You can't divide by zero.")
except ValueError:
    print("That's not a number!")
else:
    print("Your result is:", result)
finally:
    print("This will run no matter what.")
```  nn





<table>
  <tr>
    <th>Exception</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>ArithmeticError</td>
    <td>Raised when an error occurs in numeric calculations</td>
    <td><code>1 / 0</code></td>
  </tr>
  <tr>
    <td>AssertionError</td>
    <td>Raised when an assert statement fails</td>
    <td><code>assert 1 == 2</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>AttributeError</td>
    <td>Raised when attribute reference or assignment fails</td>
    <td><code>'hello'.non_existing_method()</code></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Base class for all exceptions</td>
    <td>Custom exceptions inherit from <code>Exception</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>EOFError</td>
    <td>Raised when the input() method hits an "end of file" condition (EOF)</td>
    <td><code>input()</code> with no input in an interactive session</td>
  </tr>
  <tr>
    <td>FloatingPointError</td>
    <td>Raised when a floating point calculation fails</td>
    <td><code>float('inf') - float('inf')</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>GeneratorExit</td>
    <td>Raised when a generator is closed (with the close() method)</td>
    <td><code>gen = (i for i in range(10))<br>gen.close()</code></td>
  </tr>
  <tr>
    <td>ImportError</td>
    <td>Raised when an imported module does not exist</td>
    <td><code>import non_existing_module</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>IndentationError</td>
    <td>Raised when indentation is not correct</td>
    <td><code>def func():<br>return 1</code> (incorrect indentation)</td>
  </tr>
  <tr>
    <td>IndexError</td>
    <td>Raised when an index of a sequence does not exist</td>
    <td><code>[1, 2, 3][5]</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>KeyError</td>
    <td>Raised when a key does not exist in a dictionary</td>
    <td><code>{'a': 1}['b']</code></td>
  </tr>
  <tr>
    <td>KeyboardInterrupt</td>
    <td>Raised when the user presses Ctrl+c, Ctrl+z or Delete</td>
    <td>Occurs during manual interruption</td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>LookupError</td>
    <td>Raised when errors raised can't be found</td>
    <td>Base class for <code>IndexError</code> and <code>KeyError</code></td>
  </tr>
  <tr>
    <td>MemoryError</td>
    <td>Raised when a program runs out of memory</td>
    <td>Creating an extremely large list (e.g., <code>[0] * 10**10</code>)</td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>NameError</td>
    <td>Raised when a variable does not exist</td>
    <td><code>print(unknown_variable)</code></td>
  </tr>
  <tr>
    <td>NotImplementedError</td>
    <td>Raised when an abstract method requires an inherited class to override the method</td>
    <td><code>class MyClass:<br> def method(self):<br> raise NotImplementedError()</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>OSError</td>
    <td>Raised when a system-related operation causes an error</td>
    <td><code>open('non_existing_file.txt')</code></td>
  </tr>
  <tr>
    <td>OverflowError</td>
    <td>Raised when the result of a numeric calculation is too large</td>
    <td><code>float('inf') * 10**308</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>ReferenceError</td>
    <td>Raised when a weak reference object does not exist</td>
    <td><code>import weakref<br> weakref.ref()</code></td>
  </tr>
  <tr>
    <td>RuntimeError</td>
    <td>Raised when an error occurs that does not belong to any specific exceptions</td>
    <td><code>raise RuntimeError('An error occurred')</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>StopIteration</td>
    <td>Raised when the next() method of an iterator has no further values</td>
    <td><code>next(iter([]))</code></td>
  </tr>
  <tr>
    <td>SyntaxError</td>
    <td>Raised when a syntax error occurs</td>
    <td><code>eval('x === 1')</code> (invalid syntax)</td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>TabError</td>
    <td>Raised when indentation consists of tabs or spaces</td>
    <td>Mixing tabs and spaces in Python code</td>
  </tr>
  <tr>
    <td>SystemError</td>
    <td>Raised when a system error occurs</td>
    <td>Internal Python interpreter error</td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>SystemExit</td>
    <td>Raised when the sys.exit() function is called</td>
    <td><code>import sys<br>sys.exit()</code></td>
  </tr>
  <tr>
    <td>TypeError</td>
    <td>Raised when two different types are combined</td>
    <td><code>'1' + 1</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>UnboundLocalError</td>
    <td>Raised when a local variable is referenced before assignment</td>
    <td><code>def func():<br> print(x)<br> x = 1</code></td>
  </tr>
  <tr>
    <td>UnicodeError</td>
    <td>Raised when a Unicode problem occurs</td>
    <td>Base class for <code>UnicodeEncodeError</code>, <code>UnicodeDecodeError</code>, etc.</td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>UnicodeEncodeError</td>
    <td>Raised when a Unicode encoding problem occurs</td>
    <td><code>'é'.encode('ascii')</code></td>
  </tr>
  <tr>
    <td>UnicodeDecodeError</td>
    <td>Raised when a Unicode decoding problem occurs</td>
    <td><code>b'\x80abc'.decode('utf-8')</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>UnicodeTranslateError</td>
    <td>Raised when a Unicode translation problem occurs</td>
    <td><code>'é'.encode('latin-1').decode('utf-8')</code></td>
  </tr>
  <tr>
    <td>ValueError</td>
    <td>Raised when there is a wrong value in a specified data type</td>
    <td><code>int('abc')</code></td>
  </tr>
  <tr style="background-color: #e0f7ff;">
    <td>ZeroDivisionError</td>
    <td>Raised when the second operator in a division is zero</td>
    <td><code>1 / 0</code></td>
  </tr>
</table>
````
