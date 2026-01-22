# Debug
- [Debug Print](#Debug-Print)
    - [Literals](#Literals)
    - [Variables](#Variables)
    - [Expressions](#Expressions)
    - [Array](#Array)
- [Debug Assert](#Debug-Assert)
- 
&nbsp;
## Debug Print
> ### Literals
```vba
Sub DebugPrintLiteral()
    Debug.Print 1
    Debug.Print "Hello World"
    Debug.Print 3.14
    Debug.Print True
End Sub
```
```vba
 1 
Hello World
 3,14 
True
```
> ### Variables
```vba
Sub DebugPrintVariable()
    Dim x As Integer
    Dim name As String
    Dim pi As Double
    Dim isValid As Boolean
    
    x = 10
    name = "Excel"
    pi = 3.14159
    isValid = False
    
    Debug.Print x
    Debug.Print name
    Debug.Print pi
    Debug.Print isValid
End Sub
```
```vba
 10 
Excel
 3,14159 
False
```
> ### Expressions
```vba
Sub DebugPrintExpressions()
    Dim a As Integer, b As Integer
    a = 5
    b = 3

    Debug.Print a, b
    Debug.Print a + b
    Debug.Print a * b
    Debug.Print "Sum: " & (a + b)
    Debug.Print "Product: " & (a * b)
End Sub
```
```vba
 5             3
 8
 15
Sum: 8
Product: 15
```
> ### Array
```vba
Sub DebugPrintArray()
    Dim arr(1 To 3) As Integer
    Dim i As Integer
    arr(1) = 5
    arr(2) = 10
    arr(3) = 20
    
    For i = 1 To 3 Step 1
        Debug.Print "Element " & i & " = " & arr(i)
    Next i
End Sub
```
```vba
Element 1 = 5
Element 2 = 10
Element 3 = 20
```
## Debug Assert
