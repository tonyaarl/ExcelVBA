# Excel VBA Custom Functions

## Arithmetic
### Addition
```vba
Function Addition(A As Integer, B As Integer) As Integer
    Addition = A + B
End Function
```
&nbsp;
### Subtraction
```vba
Function Subtraction(A As Integer, B As Integer) As Integer
    Subtraction = A - B
End Function
```
### Multiplication
```vba
Function Multiplication(A As Integer, B As Integer) As Integer
    Multiplication = A * B
End Function
```
### Division
```vba
Function Division(A As Integer, B As Integer) As Integer
    If B = 0 Then
        Division = 0
    Else
        Division = A / B
    End If
End Function
```
