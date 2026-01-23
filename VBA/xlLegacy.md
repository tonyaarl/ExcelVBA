# Legacy
## Variables
> ### Implicit Type Declaration Characters
```vba
Sub LegacyCharacters()
    a% = 1      ' % Integer
    b& = 2      ' & Long
    c! = 3      ' ! Single
    d# = 4      ' # Double
    e$ = "5"    ' $ String
    f@ = 6      ' @ Currency
    
    Debug.Print a & b & c & d & e & f
End Sub
```
```vba
123456
```
## Statement
> ### Line Continuation
```vba
Sub LineContinuation()
    Dim x As Integer
    
    x = 1 + 2 + 3 _
    + 4 + 5
    
    Debug.Print x
End Sub
```
```vba
15
```
