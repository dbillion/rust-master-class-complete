# Mermaid Diagrams from Rust Course Code

This document shows what Mermaid diagrams can be generated from the Rust course code examples.

## 1. Flowchart - Chapter 2: Basic Programming

```mermaid
flowchart TD
    A[Start Program] --> B[Declare Variables]
    B --> C[Define Data Types]
    C --> D{Mutable?}
    D -->|Yes| E[let mut x = value]
    D -->|No| F[let x = value]
    E --> G[Use Variables]
    F --> G
    G --> H[Call Functions]
    H --> I[End Program]
    
    style A fill:#b2f2bb
    style I fill:#ffc9c9
    style D fill:#fef3c7
```

## 2. Sequence Diagram - Chapter 3: Ownership

```mermaid
sequenceDiagram
    participant Owner as Owner
    participant Borrower as Borrower
    participant Data as Data (Heap)
    
    Owner->>Data: Create String::from()
    Note over Owner,Data: Owner has exclusive access
    
    Owner->>Borrower: &self (immutable borrow)
    Note over Borrower,Data: Can read, not modify
    
    Owner->>Borrower: &mut self (mutable borrow)
    Note over Borrower,Data: Can read and modify
    
    Owner->>Data: Drop when out of scope
    Note over Data: Memory freed
```

## 3. Class Diagram - Chapter 6: Structs & Traits

```mermaid
classDiagram
    class Shape {
        +String color
        +f64 area
        +calculateArea() f64
        +describe() String
    }
    
    class Rectangle {
        +f64 width
        +f64 height
        +new(w, h) Rectangle
        +area() f64
    }
    
    class Circle {
        +f64 radius
        +new(r) Circle
        +area() f64
    }
    
    class Drawable {
        <<interface>>
        +draw()
        +render()
    }
    
    Shape <|-- Rectangle
    Shape <|-- Circle
    Drawable <|.. Rectangle
    Drawable <|.. Circle
```

## 4. State Diagram - Chapter 4: Control Structures

```mermaid
stateDiagram-v2
    [*] --> Start
    Start --> IfCheck: Evaluate condition
    IfCheck --> IfBlock: condition = true
    IfCheck --> ElseBlock: condition = false
    IfBlock --> EndIf
    ElseBlock --> EndIf
    EndIf --> MatchExpr
    MatchExpr --> Pattern1: matches pattern 1
    MatchExpr --> Pattern2: matches pattern 2
    MatchExpr --> Wildcard: default (_)
    Pattern1 --> End
    Pattern2 --> End
    Wildcard --> End
    End --> [*]
```

## 5. ER Diagram - Chapter 8: Modules

```mermaid
erDiagram
    CRATE ||--o{ MODULE : contains
    MODULE ||--o{ ITEM : exports
    MODULE ||--o{ MODULE : nested
    
    CRATE {
        string name
        string type "lib/main"
    }
    
    MODULE {
        string visibility "pub/private"
        string path
    }
    
    ITEM {
        string type "fn/struct/trait"
        string visibility
    }
```

## 6. Git Graph - Chapter 5: Stack Project

```mermaid
gitGraph
    commit id: "Initial: Stack struct"
    commit id: "Add push method"
    commit id: "Add pop method"
    branch string-reversal
    checkout string-reversal
    commit id: "Implement reversal"
    commit id: "Add tests"
    checkout main
    merge string-reversal
    commit id: "Documentation"
```

## 7. Mindmap - Chapter 14: Concurrency

```mermaid
mindmap
  root((Concurrency))
    Threads
      spawn
      join
      move closure
    Communication
      Channels
        mpsc
        send/recv
      Shared State
        Mutex
        Arc
        RwLock
    Async
      async fn
      .await
      Futures
    Safety
      Send trait
      Sync trait
      Atomic types
```

## 8. Gantt Chart - Course Timeline

```mermaid
gantt
    title Rust Master Class Timeline
    dateFormat  YYYY-MM-DD
    section Basics
    Chapter 2: Basic Programming :done, ch2, 2024-01-01, 7d
    Chapter 3: Ownership :done, ch3, after ch2, 5d
    Chapter 4: Control Structures :done, ch4, after ch3, 5d
    section Intermediate
    Chapter 5: Stack Project :active, ch5, after ch4, 7d
    Chapter 6-9: Advanced Topics : ch6, after ch5, 14d
    section Advanced
    Chapter 14: Concurrency : ch14, after ch6, 10d
    Chapter 24: Blockchain : ch24, after ch14, 14d
```

## 9. Journey Diagram - Learning Path

```mermaid
journey
    title Learning Rust Journey
    section Foundation
      Learn Variables: 5: Student
      Understand Ownership: 3: Student
      Master Control Flow: 4: Student
    section Practice
      Build Stack Project: 5: Student, Mentor
      Implement Traits: 4: Student
    section Advanced
      Concurrency Patterns: 3: Student
      Build Blockchain: 5: Student, Mentor
    section Mastery
      Web Programming: 4: Student
      Performance Optimization: 5: Student
```

## 10. Timeline - Chapter 7: Lifetimes

```mermaid
timeline
    title Lifetime of References
    section Function Start
        Parameter x received : 'a
        Parameter y received : 'a
    section Function Body
        Use x : 'a still valid
        Use y : 'a still valid
    section Function End
        Return value : 'a ends
        Drop parameters
```

## 11. C4 Container Diagram - Chapter 25: Web Programming

```mermaid
C4Container
    title Web Application Architecture
    
    Person(user, "User", "Web browser user")
    
    Container_Boundary(web_app, "Web Application") {
        Container(frontend, "Frontend", "Rust + WebAssembly", "Handles UI and user interactions")
        Container(backend, "Backend API", "Rust + Actix", "REST API and business logic")
        ContainerDb(database, "Database", "PostgreSQL", "Stores user data and content")
    }
    
    Rel(user, frontend, "Uses", "HTTPS")
    Rel(frontend, backend, "Calls", "JSON/HTTP")
    Rel(back, database, "Reads/Writes", "SQL")
```

## 12. Pie Chart - Chapter 2: Data Types Distribution

```mermaid
pie title Rust Data Types Usage
    "Integers (i32, u32)" : 40
    "Floats (f64)" : 20
    "Boolean" : 15
    "Characters" : 10
    "Strings" : 15
```

---

## How to Generate These with Mermaid MCP

Once installed, the Mermaid MCP server would provide tools like:

```bash
# Generate SVG from Mermaid code
mcp-cli call mermaid generate_svg '{"code": "flowchart TD\\nA --> B", "output": "diagram.svg"}'

# Generate PNG
mcp-cli call mermaid generate_png '{"code": "sequenceDiagram\\nAlice->>Bob", "output": "diagram.png"}'

# Validate syntax
mcp-cli call mermaid validate '{"code": "flowchart TD\\nA -->"}'
```

## Integration with Rust Course

Each chapter can have:
1. **Flowcharts** for code logic
2. **Sequence diagrams** for ownership/borrowing
3. **Class diagrams** for structs and traits
4. **State diagrams** for control flow
5. **Mindmaps** for concept organization
6. **Gantt charts** for project timelines
7. **Journey diagrams** for learning paths
