# Rust Programming Master Class - Excalidraw Diagrams

This directory contains visual infographics for each chapter of the Rust Programming Master Class.

## Created Diagrams

| Chapter | Topic | File | Status |
|---------|-------|------|--------|
| 2 | Basic Programming | `chapter_02_basic_programming.excalidraw.json` | ✅ Created |
| 3 | Rust Ownership | `chapter_03_ownership.excalidraw.json` | ✅ Created |
| 4 | Control Structures | `chapter_04_control_structures.excalidraw.json` | ✅ Created |
| 5 | Project: Stack Implementation | `chapter_05_stack.excalidraw.json` | ✅ Created |
| 6 | Structures, Traits, Generics, Enums | `chapter_06_structs_traits_generics_enums.excalidraw.json` | ✅ Created |
| 7 | Iterators, Lifetimes, Closures | `chapter_07_iterators_lifetimes_closures.excalidraw.json` | ✅ Created |
| 8 | Rust Modules | `chapter_08_modules.excalidraw.json` | ✅ Created |
| 9 | Smart Pointers | `chapter_09_smart_pointers.excalidraw.json` | ✅ Created |
| 10 | Advance Techniques | `chapter_10_advance.excalidraw.json` | ⏳ Pending |
| 11 | Real Life Application | `chapter_11_real_life.excalidraw.json` | ⏳ Pending |
| 12 | Deep Dive into Traits | `chapter_12_traits.excalidraw.json` | ⏳ Pending |
| 13 | Efficient Programming | `chapter_13_efficient.excalidraw.json` | ⏳ Pending |
| 14 | Concurrency in Rust | `chapter_14_concurrency.excalidraw.json` | ✅ Created |
| 15 | Text Processing, File & Directory | `chapter_15_text_processing.excalidraw.json` | ⏳ Pending |
| 16 | Sized and Unsized Types | `chapter_16_sized_types.excalidraw.json` | ⏳ Pending |
| 17 | Error Handling | `chapter_17_error_handling.excalidraw.json` | ⏳ Pending |
| 18 | Beyond Basic References | `chapter_18_references.excalidraw.json` | ⏳ Pending |
| 19 | Coercion in Rust | `chapter_19_coercion.excalidraw.json` | ⏳ Pending |
| 20 | Beyond Simple Lifetimes | `chapter_20_lifetimes.excalidraw.json` | ⏳ Pending |
| 21 | Traits | `chapter_21_traits.excalidraw.json` | ⏳ Pending |
| 22 | Downcasting | `chapter_22_downcasting.excalidraw.json` | ⏳ Pending |
| 23 | Dropcheck | `chapter_23_dropcheck.excalidraw.json` | ⏳ Pending |
| 24 | BlockChain from Scratch | `chapter_24_blockchain.excalidraw.json` | ⏳ Pending |
| 25 | Web Programming | `chapter_25_web.excalidraw.json` | ⏳ Pending |
| 26 | Measuring & Improving Performance | `chapter_26_performance.excalidraw.json` | ⏳ Pending |

## How to View Diagrams

### Option 1: Import to Excalidraw
1. Go to https://excalidraw.com
2. Click "Open" → "Load" 
3. Select the `.excalidraw.json` file
4. View and interact with the diagram

### Option 2: Use Excalidraw MCP
```bash
# Using mcp-cli
mcp-cli call excalidraw create_view \
  '{"elements": "$(cat chapter_02_basic_programming.excalidraw.json | jq -r \".elements\")"}'
```

### Option 3: Render to PNG
```bash
cd /path/to/excalidraw-mcp-app
npm run render ../diagrams/chapter_02_basic_programming.excalidraw.json
```

## Diagram Design Principles

Each diagram follows these principles:
- **Visual Argument**: Shows relationships, not just boxes
- **Multi-Zoom**: Summary flow + section boundaries + detailed examples
- **Evidence Artifacts**: Includes actual code snippets
- **Color-Coded**: Consistent color scheme for different concepts
- **Clean Aesthetics**: Modern, professional look with roughness=0

## Color Scheme

| Color | Usage |
|-------|-------|
| Blue (#a5d8ff) | Titles, inputs, sources |
| Green (#b2f2bb) | Success, outputs, completed |
| Orange (#ffd8a8) | Warnings, external, processing |
| Purple (#d0bfff) | Advanced concepts, middleware |
| Red (#ffc9c9) | Errors, critical items |
| Yellow (#fff3bf) | Decisions, notes |
| Teal (#c3fae8) | Data, storage |

## Next Steps

- [ ] Create remaining 17 chapter diagrams
- [ ] Add cross-chapter concept maps
- [ ] Create summary diagrams for major sections
- [ ] Export all diagrams to PNG for documentation

---
Generated: 2026-03-30
