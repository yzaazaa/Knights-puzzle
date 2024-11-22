# Knights and Knaves Puzzle Solver

## Description
This project focuses on knowledge engineering - the process of translating natural language statements into formal logical representations. Using Knights and Knaves puzzles inspired by Raymond Smullyan's 1978 book "What is the name of this book?".

## Learning Objectives
- Practice knowledge engineering by translating English sentences into propositional logic using my logical inference engine
- Understand how to build and maintain logical knowledge bases
- Apply model checking algorithms to verify logical conclusions
- Gain experience with formal logical reasoning and inference

## Background
In these puzzles:
- Each character is either a knight or a knave
- Knights always tell the truth
- Knaves always lie
- The goal is to determine each character's identity based on their statements

The key challenge is not solving the puzzles directly, but rather expressing the puzzle constraints and statements in proper logical form that can be programmatically verified.

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yzaazaa/knights-puzzle
cd knights-puzzle
```

2. Run the script:
```bash
python puzzle.py
```

## Knowledge Engineering Process
1. Understand the given statements in natural language
2. Identify the logical implications of each statement
3. Translate statements into propositional logic using provided logical operators
4. Build a knowledge base combining all logical statements
5. Use model checking to verify possible solutions

## Puzzles Included

### Puzzle 0
Single character puzzle:
- Character A says: "I am both a knight and a knave."
- Knowledge engineering task: Express this statement and its implications in propositional logic

### Puzzle 1
Two character puzzle:
- Character A says: "We are both knaves."
- Character B says nothing.
- Knowledge engineering task: Express A's statement while accounting for B's presence

### Puzzle 2
Two character puzzle:
- Character A says: "We are the same kind."
- Character B says: "We are of different kinds."
- Knowledge engineering task: Express these contradictory statements in logic

### Puzzle 3
Three character puzzle:
- Character A says either "I am a knight." or "I am a knave." (unknown which)
- Character B says: "A said 'I am a knave.'"
- Character B also says: "C is a knave."
- Character C says: "A is a knight."
- Knowledge engineering task: Express complex nested statements and uncertain claims

## Implementation Details
The project uses propositional logic to represent the puzzles. Each character's status (knight or knave) is represented as a logical proposition, and their statements are converted into logical expressions. The program then uses model checking to determine which combinations of knight/knave assignments are consistent with all statements.

### Key Components
- **Logical Operators**: And, Or, Not, Implication, Bicondition
- **Knowledge Base**: Collection of logical sentences representing puzzle constraints
- **Model Checking**: Algorithm to verify logical conclusions

## Key Files
- `logic.py`: Contains classes for logical connectives and the model checking algorithm
- `puzzle.py`: Contains the puzzle definitions and knowledge bases for each puzzle

## Requirements
- Python 3.7+
- No external dependencies
