# Reverse Engineering Fundamentals

## Description

This project introduces the fundamental concepts and practical skills required for reverse engineering binary files. Students learn to analyze ELF executables, identify unusual sections, and map external library dependencies using standard Linux analysis tools.


## Project Tasks

### Task 0: ELF Header Analysis
**File**: `get_entry_point.sh`
- Create a Bash script to extract ELF header information
- Extract magic number, class, byte order, and entry point address
- Implement error handling and input validation

### Task 1: Section Enumeration
**Files**: `size.txt`, `command.txt`
- Analyze binary sections using `readelf -S` or `objdump -h`
- Identify unusual sections (non-standard names)
- Document the size of suspicious sections

### Task 2: External Library Dependencies
**File**: `external_library.txt`
- Use `ldd` to identify external library dependencies
- Distinguish between system libraries and custom/external libraries
- Document non-standard library dependencies

## Usage

### ELF Header Analysis
```bash
chmod +x get_entry_point.sh
./get_entry_point.sh task0
```

### Section Analysis
```bash
readelf -S task1
# Document unusual section size in size.txt
```

### Library Dependencies
```bash
ldd task2
# Document external libraries in external_library.txt
```
