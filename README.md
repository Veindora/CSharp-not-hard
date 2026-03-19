# SIT232 Practical Tasks 1.1P & 1.2P: Selection, Casting, and Repetition

This repository contains the implementation of Practical Tasks 1.1P and 1.2P for SIT232 (Object-Oriented Development). These tasks focus on C# control structures, including selection (`if`, `switch`), casting, and repetition (`for`, `while`, `do...while` loops).

## Project Structure

### Practical Task 1.1P: Selection and Casting (`selection_and_casting/`)
- **`IfStatement/`**: Implementation of Task 1, converting numbers 1-9 to words using `if-else` blocks.
- **`SwitchStatement/`**: Implementation of Task 2, using `switch` statements for the same number-to-word conversion.
- **`Microwave/`**: Task 5, calculating heating times based on the number of items.
- **`DoCasting/`**: Task 6, demonstrating explicit casting and its effect on division results.
- **`Analysis.md`**: Detailed analysis and fixes for the Task 3 and 4 code snippets.
- **`task/`**: Standalone fixed C# files for the debugging snippets in Tasks 3 and 4 (`Snippet1.cs` to `Snippet8.cs`).

### Practical Task 1.2P: Repetition (`repetition/`)
- **`Repetition.cs`**: Implements Tasks 1, 2, and 3. Calculates the sum and average of numbers 1 to 100 using all three loop types.
- **`DebuggingAndRewriting.cs`**: Implements logic for Task 4 (debugging) and Task 5 (rewriting `while` loops as `for` loops).
- **`GuessingNumber.cs`**: A two-player number guessing game with input validation (Task 6).
- **`DivisibleFour.cs`**: Finds numbers divisible by 4 but not by 5 up to a user limit (Task 7).
- **`analyze.md`**: Theoretical answers regarding loop differences and a breakdown of Task 4 bugs.
- **`task/`**: Standalone fixed C# files for the debugging snippets in Task 4 (`Snippet1.cs` to `Snippet7.cs`).

## Repository Structure

```text
.
├── 1.1P_request.pdf          # Task 1.1P requirements
├── 1.2P_request.pdf          # Task 1.2P requirements
├── README.md                 # Project documentation
├── selection_and_casting/    # Task 1.1P implementation
│   ├── Analysis.md           # Analysis for Task 3 & 4
│   ├── DoCasting/
│   ├── IfStatement/
│   ├── Microwave/
│   ├── SwitchStatement/
│   └── task/                 # Fixed debugging snippets (Task 3 & 4)
│       ├── Snippet1.cs to Snippet8.cs
└── repetition/               # Task 1.2P implementation
    ├── analyze.md            # Analysis for Task 4
    ├── DebuggingAndRewriting.cs
    ├── DivisibleFour.cs
    ├── GuessingNumber.cs
    ├── Repetition.cs
    └── task/                 # Fixed debugging snippets (Task 4)
        ├── Snippet1.cs to Snippet7.cs
```

## Highlights & Key Takeaways
> [!NOTE]
> The **`do...while`** loop is used for the user input section in Task 6 because it guarantees that the prompt will be displayed at least once, regardless of the initial condition.

> [!IMPORTANT]
> All user inputs are validated using **`int.TryParse`**. This prevents the application from crashing if a user enters non-numeric text, ensuring a robust and user-friendly experience.

> [!TIP]
> **What is the fundamental difference between a `while` and a `for` loop?**
> A `for` loop is most effective when the number of iterations is known (fixed-count), while a `while` loop is better suited for condition-based iterations where the count is not predetermined.

## Implementation Process

1.  **Requirement Analysis**: Analyzed the provided PDF to extract specific logic requirements and output formatting constraints.
2.  **Loop Implementation**: Built the core repetition logic, ensuring `do...while` loops were used correctly for scenarios requiring at least one execution (like input validation).
3.  **Debugging Phase**: Identified common logic errors in provided snippets, such as:
    - Infinite loops caused by parity mismatches.
    - Variable scope issues (internal re-declaration).
    - Uninitialized variables.
    - Syntax errors in `for` loop headers.
4.  **Refactoring**: Demonstrated the conversion of `while` loops into more concise `for` loops where appropriate.
5.  **Validation**: Added input handling (using `int.TryParse`) to ensure the programs are robust against invalid user entries.

## How to Run
To compile and run any of these files, use the .NET CLI:
```bash
csc FileName.cs
.\FileName.exe
```
*(Note: Ensure you have the .NET SDK or Build Tools installed.)*
