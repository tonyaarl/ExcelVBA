# Excel VBA Native Functions

## Debug Functions

### Debug.Print
```vba
Sub DebugPrintLiteral()
    Debug.Print 1
    Debug.Print "Hello World"
    Debug.Print 3.14
End Sub
```
```vba
Sub DebugPrintVariable()
    Dim x As Integer
    Dim name As String
    Dim pi As Double
    
    x = 10
    name = "Excel"
    pi = 3.14159
    
    Debug.Print x
    Debug.Print name
    Debug.Print pi
End Sub
```
```vba
Sub DebugPrintExpressions()
    Dim a As Integer, b As Integer
    a = 5
    b = 3
    
    Debug.Print a + b
    Debug.Print a * b
    Debug.Print "Sum: " & (a + b)
    Debug.Print "Product: " & (a * b)
End Sub
```
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
Sub DebugPrintMixed()
    Dim x As Integer
    Dim msg As String
    
    x = 7
    msg = "Lucky number is:"
    
    Debug.Print msg, x
End Sub
```
