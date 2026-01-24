# Main Title

- [Section][#Section]

## Section
### Subsection




# Legacy
- [Variables](#Variables)
    - [Implicit Type Declaration Characters](#Implicit-Type-Declaration-Characters)
    - [Implicit Module Declaration Statement](#Implicit-Module-Declaration-Statement)
- [Statement](#Statement)
- [Procedure Invocation](#Procedure-Invocation)
- [Control Flow](#Control-Flow)
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
- Disabled By: [Option Explicit](xlSyntax.md#Force-Variable-Declaration)
> ### Implicit Module Declaration Statement
```vba
DefInt A-C
DefBool D-F
DefStr M-O, W

Sub Define()

    a = 1
    b = 2
    c = 3
    
    d = True
    e = True
    f = False
    
    m = "He"
    n = "ll"
    o = "o"
    w = "World!"

    Debug.Print a + b + c
    Debug.Print d, e, f
    Debug.Print m & n & o & " " & w

End Sub
```
```vba
 6 
True          True          False
Hello World!
```
- Disabled By: [Option Explicit](xlSyntax.md#Force-Variable-Declaration)
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
## Procedure Invocation
> ### Call
```vba
Sub ProcedureInvocation()
    Call Foo
    Bar
End Sub

Function Foo()
    Debug.Print "Hello"
End Function

Function Bar()
    Debug.Print "World"
End Function
```
```vba
Hello
World
```
## Control Flow
> ### GoSub
```vba
Sub ControlFlow()

    Debug.Print "Step 1"
    GoSub MyLabel
    Debug.Print "Step3"
    Exit Sub
    
MyLabel:
    Debug.Print "Step 2"
    Return

End Sub
```
