# Diagram Guideline


## Flowchart
```mermaid
graph TD
    A[Start] --> B{Decision}
    B -- Yes --> C[Do it]
    B -- No --> D[Skip]
    C --> E[End]
    D --> E
```
## Sequence Diagram
```mermaid
sequenceDiagram
    Alice->>Bob: Hello Bob
    Bob-->>Alice: Hi Alice
```
## Class Diagram
```mermaid
classDiagram
    class Dog {
        +name
        +bark()
    }
    class Owner {
        +name
    }
    Owner --> Dog
```
## State Diagram
```mermaid
stateDiagram-v2
    [*] --> Idle
    Idle --> Running : start
    Running --> Idle : stop
```
## Entity-Relationship Diagram
```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE_ITEM : contains
    PRODUCT ||--o{ LINE_ITEM : referenced_by
```
## Gantt Chart
```mermaid
gantt
    title Project Timeline
    dateFormat  YYYY-MM-DD
    section Planning
    Specs       :a1, 2026-02-01, 5d
    Review      :after a1, 2d
```
## Pie Chart
```mermaid
pie
    title Bug Distribution
    "UI" : 40
    "Backend" : 35
    "Docs" : 25
```
## User Journey
```mermaid
journey
    title User Onboarding
    section Sign Up
      Fill form: 5: User
      Confirm email: 3: User
    section First Login
      Tour app: 2: User
```
## Mindmap
```mermaid
mindmap
  root((Project))
    Docs
      Style Guide
      Mermaid
    Code
      Excel
      Macros
```
## Timeline
```mermaid
timeline
    title Project Milestones
    2026-01-01 : Project Start
    2026-02-01 : First Prototype
    2026-03-01 : Beta Release
```
