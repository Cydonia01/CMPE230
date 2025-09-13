# CMPE230 - Computer Engineering Projects

This repository contains two comprehensive C programming projects developed for the CMPE230 Computer Engineering course. The projects demonstrate advanced programming concepts including parsing, execution engines, stack-based algorithms, and assembly language programming.

_These projects were implemented with the cooperation of SuleymanTolgaAcar._

## Projects Overview

### 1. Favor for the Ringmaster (Project 1)

An interactive inventory management system that processes natural language commands to manage subjects, items, and locations. The program features a sophisticated parsing engine and conditional execution system.

**Key Features:**

- Natural language command parsing
- Dynamic inventory management for multiple subjects
- Conditional execution with two-pointer evaluation algorithm
- Interactive terminal-based interface
- Real-time transaction processing

**Technologies:** C, Dynamic memory management, String parsing, Conditional logic

### 2. Postfix Translator (Project 2)

A postfix expression evaluator that translates mathematical expressions into RISC-V assembly instructions. Implements stack-based evaluation and binary conversion algorithms.

**Key Features:**

- Postfix expression evaluation using assembly stack operations
- Decimal to binary number conversion
- RISC-V instruction generation
- Support for arithmetic and logical operations (+, -, \*, XOR, AND, OR)

**Technologies:** RISC-V Assembly, Stack-based algorithms, Binary operations

## Quick Start

### Prerequisites

- GCC compiler
- Make build system
- Python 3.x (for testing)

### Building Projects

Navigate to either project directory and compile:

```bash
# For Favor for the Ringmaster
cd "Favor for the Ringmaster"
make

# For Postfix Translator
cd "Postfix Translator"
make
```

### Running Projects

```bash
# Favor for the Ringmaster
./ringmaster

# Postfix Translator
./postfix_translator
```

### Testing

Both projects include comprehensive test suites with automated grading:

```bash
# Run tests for either project
make grade

# Or manually with Python
python test/grader.py ./[executable_name] test-cases
```

## Project Structure

```
CMPE230/
├── Readme.md                          # This file
├── Favor for the Ringmaster/           # Project 1
│   ├── Makefile                       # Build configuration
│   ├── README.md                      # Detailed project documentation
│   ├── src/                           # Source code
│   │   ├── ringmaster.c              # Main program file
│   │   ├── inventory.h               # Inventory management system
│   │   └── execute.h                 # Execution engine
│   ├── docs/                         # Documentation
│   │   ├── description.pdf           # Project specification
│   │   ├── description.tex           # LaTeX source
│   │   └── tolkien.jpeg              # Reference image
│   ├── test/                         # Testing framework
│   │   ├── checker.py                # Test validation
│   │   └── grader.py                 # Automated grading
│   └── test-cases/                   # Test input/output files
│       ├── input_*.txt               # Test inputs
│       └── output_*.txt              # Expected outputs
└── Postfix Translator/                # Project 2
    ├── Makefile                       # Build configuration
    ├── README.md                      # Detailed project documentation
    ├── description.pdf                # Project specification
    ├── src/                           # Source code
    │   └── postfix_translator.s       # Assembly implementation
    ├── test/                          # Testing framework
    │   ├── checker.py                 # Test validation
    │   └── grader.py                  # Automated grading
    └── test-cases/                    # Test input/output files
        ├── input_*.txt                # Test inputs
        └── output_*.txt               # Expected outputs
```

## Technical Implementation

### Favor for the Ringmaster

- **Parsing Engine:** State-based tokenization with context-aware parsing
- **Execution Model:** Two-pointer condition evaluation algorithm
- **Memory Management:** Dynamic allocation with proper cleanup
- **Data Structures:** Operation structs, inventory arrays, subject tracking

### Postfix Translator

- **Stack Operations:** Assembly-level stack manipulation
- **Number Conversion:** Character-to-decimal and decimal-to-binary algorithms
- **Instruction Generation:** RISC-V assembly output formatting
- **Operation Support:** Arithmetic and logical operators
