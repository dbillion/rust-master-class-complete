# 📊 Rust Course Diagrams - Complete Collection

Comprehensive Mermaid diagrams organized by chapter for the Rust Programming Master Class.

---

## 🎯 Quick Navigation

### By Chapter

| Chapter | Topic | Diagrams | Location |
|---------|-------|----------|----------|
| **00** | Overview | 1 Git Graph | [`ch00-overview/`](./by-chapter/ch00-overview/) |
| **02** | Basics | 3 diagrams | [`ch02-basics/`](./by-chapter/ch02-basics/) |
| **03** | Ownership | 3 diagrams | [`ch03-ownership/`](./by-chapter/ch03-ownership/) |
| **04** | Control | 3 diagrams | [`ch04-control/`](./by-chapter/ch04-control/) |
| **05** | Stack Project ⭐ | 4 diagrams (C4) | [`ch05-stack-project/`](./by-chapter/ch05-stack-project/) |
| **06** | Structs & Traits | 2 diagrams | [`ch06-structs-traits/`](./by-chapter/ch06-structs-traits/) |
| **07** | Iterators & Lifetimes | 2 diagrams | [`ch07-iterators-lifetimes/`](./by-chapter/ch07-iterators-lifetimes/) |
| **08** | Modules | 2 diagrams | [`ch08-modules/`](./by-chapter/ch08-modules/) |
| **09** | Smart Pointers | 2 diagrams | [`ch09-smart-pointers/`](./by-chapter/ch09-smart-pointers/) |
| **10** | Advance Techniques | 3 diagrams | [`ch10-advance/`](./by-chapter/ch10-advance/) |
| **11** | Real Life Application | 2 diagrams | [`ch11-real-life/`](./by-chapter/ch11-real-life/) |
| **12** | Deep Dive into Traits | 1 diagram | [`ch12-traits-deep/`](./by-chapter/ch12-traits-deep/) |
| **13** | Efficient Programming | 1 diagram | [`ch13-efficient/`](./by-chapter/ch13-efficient/) |
| **14** | Concurrency | 3 diagrams | [`ch14-concurrency/`](./by-chapter/ch14-concurrency/) |
| **15** | Text & File Handling | 1 diagram | [`ch15-text-file/`](./by-chapter/ch15-text-file/) |
| **16** | Sized & Unsized Types | 1 diagram | [`ch16-sized-unsized/`](./by-chapter/ch16-sized-unsized/) |
| **17** | Error Handling | 2 diagrams | [`ch17-error-handling/`](./by-chapter/ch17-error-handling/) |
| **18** | References Deep Dive | 1 diagram | [`ch18-references/`](./by-chapter/ch18-references/) |
| **19** | Coercion | 1 diagram | [`ch19-coercion/`](./by-chapter/ch19-coercion/) |
| **20** | Lifetimes Deep Dive | 1 diagram | [`ch20-lifetimes-deep/`](./by-chapter/ch20-lifetimes-deep/) |
| **21** | Advanced Traits | 1 diagram | [`ch21-traits/`](./by-chapter/ch21-traits/) |
| **22** | Downcasting | 1 diagram | [`ch22-downcasting/`](./by-chapter/ch22-downcasting/) |
| **23** | Dropcheck | 1 diagram | [`ch23-dropcheck/`](./by-chapter/ch23-dropcheck/) |
| **24** | Blockchain ⭐ | 4 diagrams (C4) | [`ch24-blockchain/`](./by-chapter/ch24-blockchain/) |

**TOTAL: 46 diagrams across 24 chapters (100% coverage!)**

---

## 📁 Folder Structure

```
diagrams/
├── README.md                          # This file
├── by-chapter/                        # Organized by chapter
│   ├── ch00-overview/
│   │   └── course_git_history.mmd
│   ├── ch02-basics/
│   │   ├── 01_program_flow.mmd
│   │   ├── 02_data_types.mmd
│   │   └── 03_functions.mmd
│   ├── ch03-ownership/
│   │   ├── 01_ownership_flow.mmd
│   │   ├── 02_borrowing.mmd
│   │   └── 03_stack_heap.mmd
│   ├── ch04-control/
│   │   ├── 01_if_else_match.mmd
│   │   ├── 02_loops.mmd
│   │   └── 03_pattern_matching.mmd
│   ├── ch05-stack-project/           # ⭐ Complete project docs
│   │   ├── 01_c4_context.mmd
│   │   ├── 02_c4_container.mmd
│   │   ├── 03_c4_component.mmd
│   │   └── 04_push_pop_sequence.mmd
│   ├── ch06-structs-traits/
│   │   ├── 01_structs_traits_class.mmd
│   │   └── 02_generics_option_result.mmd
│   ├── ch07-iterators-lifetimes/
│   │   ├── 01_lifetimes_timeline.mmd
│   │   └── 02_iterator_chain.mmd
│   ├── ch08-modules/
│   │   ├── 01_module_hierarchy.mmd
│   │   └── 02_visibility_flow.mmd
│   ├── ch09-smart-pointers/
│   │   ├── 01_smart_pointer_types.mmd
│   │   └── 02_rc_reference_counting.mmd
│   ├── ch14-concurrency/
│   │   ├── 01_concurrency_overview.mmd
│   │   ├── 02_thread_spawn_join.mmd
│   │   └── 03_mpsc_channel.mmd
│   └── ch24-blockchain/              # ⭐ Complete project docs
│       ├── 01_c4_container.mmd
│       ├── 02_blockchain_class.mmd
│       ├── 03_mining_sequence.mmd
│       └── 04_git_history.mmd
│
└── mermaid/                           # Legacy - original files
    └── [original 5 diagrams]
```

---

## 🎨 Diagram Types

| Type | Count | Best For | Example |
|------|-------|----------|---------|
| **C4 Diagrams** | 6 | Project architecture | Ch05 Stack, Ch24 Blockchain |
| **Sequence** | 15 | Ownership, borrowing, function calls, drop order | Ch03, Ch05, Ch07, Ch09, Ch14, Ch15, Ch22, Ch23 |
| **Class** | 10 | Structs, traits, enums, generics, lifetimes | Ch06, Ch09, Ch12, Ch16, Ch17, Ch19, Ch20, Ch21, Ch24 |
| **Flowchart** | 13 | Control flow, decision trees, error handling | Ch02, Ch04, Ch08, Ch10, Ch11, Ch13, Ch17, Ch18 |
| **Timeline** | 1 | Lifetimes | Ch07 |
| **Mindmap** | 1 | Concept organization | Ch14 |
| **Git Graph** | 2 | Project history | Ch00, Ch24 |
| **TOTAL** | **46** | All 24 chapters | 100% coverage |

---

## 🚀 Usage

### 1. View on GitHub (Automatic Rendering)

GitHub **automatically renders** Mermaid diagrams in markdown files:

```markdown
## Ownership Flow

```mermaid
sequenceDiagram
    participant s1 as String s1
    participant s2 as String s2
    s1->>s2: s2 = s1 (MOVE)
    Note over s1: INVALIDATED!
```
```

**No image files needed!**

---

### 2. Generate SVG/PNG Locally

```bash
# Install Mermaid CLI
npm install -g @mermaid-js/mermaid-cli

# Navigate to chapter folder
cd diagrams/by-chapter/ch02-basics/

# Generate SVG
mmdc -i 01_program_flow.mmd -o 01_program_flow.svg -w 1200 -H 800

# Generate PNG
mmdc -i 01_program_flow.mmd -o 01_program_flow.png -w 1200 -H 800
```

---

### 3. Edit Diagrams

Just edit the `.mmd` text file - it's version-controlled!

```bash
# Edit diagram
vim diagrams/by-chapter/ch03-ownership/01_ownership_flow.mmd

# Commit changes
git add diagrams/by-chapter/ch03-ownership/01_ownership_flow.mmd
git commit -m "Update ownership diagram"
git push
```

---

## 📊 Featured Diagrams

### Chapter 5: Stack Project (C4 Architecture)

```mermaid
C4Context
    title Stack Project - System Context
    
    Person(developer, "Developer", "Rust programmer")
    System(stack_lib, "Stack Library", "Generic LIFO data structure")
    SystemDb(std_lib, "Rust Std Lib", "Vec<T>, Option<T>")
    
    Rel(developer, stack_lib, "Uses", "cargo add")
    Rel(stack_lib, std_lib, "Depends on", "Vec<T>")
```

---

### Chapter 24: Blockchain Mining

```mermaid
sequenceDiagram
    title Block Mining (Proof of Work)
    
    participant miner as Miner
    participant block as Block
    participant hash as HashUtil
    
    loop Mining Loop
        block->>hash: SHA256(data + nonce)
        hash-->>block: hash
        block->>block: Check: starts with "0000"?
    end
```

---

### Chapter 3: Ownership Flow

```mermaid
sequenceDiagram
    participant s1 as String s1
    participant s2 as String s2
    
    s1->>s2: s2 = s1 (MOVE)
    Note over s1: INVALIDATED!
    Note over s2: Now owns
```

---

## ✅ Git Status

**All `.mmd` files committed and pushed**  
**SVG files excluded from git** (generated on-demand)  
**Repository:** https://github.com/dbillion/rust-master-class-complete

---

## 🎯 Legend

| Symbol | Meaning |
|--------|---------|
| ⭐ | Project chapter with complete C4 documentation |
| `.mmd` | Mermaid source file (in git) |
| `.svg` | Generated SVG (local only) |
| `.png` | Generated PNG (local only) |

---

## 📖 Related Documentation

- [MERMAID_CLI_CREATED.md](./mermaid/MERMAID_CLI_CREATED.md) - Original Mermaid CLI guide
- [ALL_MERMAID_DIAGRAMS.md](../ALL_MERMAID_DIAGRAMS.md) - Complete diagram catalog
- [C4_ARCHITECTURE_PROJECTS.md](../C4_ARCHITECTURE_PROJECTS.md) - C4 diagram guide
- [LESSONS_LEARNED.md](./LESSONS_LEARNED.md) - ⭐ **Mermaid syntax pitfalls and how to avoid them**

---

## 🎓 Lessons Learned

After generating all 46 diagrams, we documented **8 common syntax errors** and their fixes:

1. ❌ **Invalid `title` statement** → Use first node for context
2. ❌ **Edge label syntax** → Labels come after target node
3. ❌ **Reserved keywords** → Avoid `option`, `opt`, `main` as participant names
4. ❌ **Special characters** → Wrap in quotes: `"pub(crate)"`
5. ❌ **Nested braces in class members** → Simplify complex signatures
6. ❌ **Multi-participant notes** → Max 2 participants per note
7. ❌ **Activate/deactivate mismatch** → Let Mermaid handle automatically
8. ❌ **Newline escapes** → Use dashes instead of `\n`

**See:** [`LESSONS_LEARNED.md`](./LESSONS_LEARNED.md) for complete guide with examples.

---

**Last Updated:** March 31, 2026
**Total Diagrams:** 46
**Chapters Covered:** 24/24 (100% coverage!)
**Status:** ✅ All .mmd files have matching .svg renders
