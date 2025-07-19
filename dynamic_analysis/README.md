# Dynamic Analysis in Reverse Engineering

A comprehensive project focused on dynamic analysis techniques in reverse engineering, covering SAT solving, anti-debugging techniques, self-modifying code, and binary analysis automation.

## Description

This project explores dynamic analysis methodologies in reverse engineering, allowing analysts to observe binary behavior during execution. Unlike static analysis, dynamic analysis provides insights into runtime behavior, system interactions, and hidden functionalities.

## Learning Objectives

By completing this project, you will be able to explain:

- Key differences between static and dynamic analysis
- Dynamic analysis techniques (breakpoints, memory dumping, execution tracing)
- Effective use of debugging tools (GDB, x64dbg, OllyDbg)
- System behavior monitoring during program execution
- Program interactions with the operating system
- Best practices for documenting dynamic analysis findings
- Real-world applications in malware analysis and security testing


## Tasks

### 0. SAT Solving in Reverse Engineering
**Objective**: Use SAT solvers to analyze logical constraints in binaries.

**Process**:
1. Disassemble binary and extract logical constraints
2. Translate constraints into Boolean formulas
3. Use Z3/MiniSat to find satisfying assignments
4. Interpret results for binary behavior analysis

**Note**: Z3 solver may require ~35 minutes execution time.

### 1. Exploring Anti-Debugging Techniques
**Objective**: Identify and bypass anti-debugging mechanisms.

**Process**:
1. Analyze binary for anti-debugging techniques
2. Document detection methods used
3. Bypass protections using debugging tools
4. Extract hidden information/flags

### 2. SAT Solving in Reverse Engineering (Advanced)
**Objective**: Advanced SAT solving techniques for complex logical constraints.

**Process**:
1. Extract complex logical constraints from binaries
2. Create Boolean formulas for SAT processing
3. Apply SAT solving to break protection mechanisms
4. Analyze results for behavioral understanding

### 3. Self-Modifying Code Analysis
**Objective**: Understand and analyze self-modifying code techniques.

**Process**:
1. Identify self-modifying code segments
2. Use dynamic analysis to decrypt modified instructions
3. Understand input validation logic
4. Extract correct input for program execution

### 4. Solve the 100 Binaries
**Objective**: Automated analysis of 100 simple arithmetic binaries.

**Challenge Details**:
- 100 binaries performing arithmetic operations (addition/subtraction)
- Each binary validates single character input
- Silent success on correct input
- Reconstruct full flag from all correct inputs

**Process**:
1. Analyze binary logic patterns
2. Identify arithmetic operations and target values
3. Automate input testing across all binaries
4. Combine results to reveal complete flag

## Best Practices

### Analysis Workflow
1. **Preparation**: Set up controlled environment and backup data
2. **Documentation**: Record all findings and methodologies
3. **Validation**: Verify results and cross-reference findings
4. **Automation**: Script repetitive tasks for efficiency

### Security Considerations
- Work in isolated environments only
- No online tools or external services
- Validate binary integrity before analysis
- Regular backups during analysis process
