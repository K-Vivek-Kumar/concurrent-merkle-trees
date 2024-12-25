# CS5300 - Final Project

**Gautham Singh (CS21BTECH11018)**  
**K Vivek Kumar (CS21BTECH11026)**

## Overview

This project implements and compares three variations of the discussed Merkle tree:

1. **Sequential Implementation**
2. **Angela et al.'s Implementation**
3. **Atomic-Update Implementation**

The source code for each implementation is included in the zip file under the following filenames:

- `Src_Prjt-cs21btech11026-sequential-merkle-tree.cpp`
- `Src_Prjt-cs21btech11026-angela-merkle-tree.cpp`
- `Src_Prjt-cs21btech11026-atomic-merkle-tree.cpp`

## Code Compilation

To compile the provided C++ source files, use the following command:

```bash
g++ Src_Prjt-cs21btech11026-<filename>.cpp -o <output>
```

For example, to compile the atomic-update implementation:

```bash
g++ Src_Prjt-cs21btech11026-atomic-merkle-tree.cpp -o atomic-merkle-tree
```

## Code Execution

Before running the compiled program, ensure that an input file named `inp.txt` is present in the same directory. This file provides the input parameters required by the program.

### Input File Format

The `inp.txt` file should contain:

1. The leaf count of the Merkle tree (`N`) and the batch size (`B`, where \(1 \leq B \leq N\)) on the first line.
2. The batch updates (of size `B`) as space-separated integers on the second line, with values ranging from \(0\) to \(N-1\).

**Example `inp.txt`:**

```
8 3
0 3 6
```

### Running the Program

After compiling, execute the generated output file. The program will automatically read the `inp.txt` file from the same directory.

```bash
./atomic-merkle-tree
```

Replace `atomic-merkle-tree` with the name of the compiled output file for other implementations.
