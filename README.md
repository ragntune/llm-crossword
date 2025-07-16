# LLM Crossword Solver Challenge

## Challenge Structure
This interview will be split into 2 sections:
- **Part 1**: 1 hour private coding time
- **Part 2**: 1 hour interview

After working on the individual coding task, you will pair program with an interviewer to discuss your solution and continue developing the crossword puzzle solver.

## Guidelines
* Try to build an efficient and fast solution
* Focus on clean, maintainable code
* Be prepared to talk about key decisions and tradeoffs
* There is no single correct solution that we are looking for
* You are not expected to complete the entire challenge, but you should be able to explain how you could get there

## Tasks

### Part 1: Individual Coding Task 
* **Time**: 60 minutes
* **AI assisted coding**: Allowed ✅ 

#### Tasks 
##### Task 1. Build an LLM powered crossword puzzle solver for `data/easy.json`

The solver should:
1. Read the clues and provide possible answers
2. Resolve any conflicting answers
3. Return a completed crossword as a result

#### Task 2. Try to extend your solution to work for the other crosswords
* The medium puzzle in `data/medium.json`
* The hard puzzle in `data/hard.json`
* The cryptic puzzle in `data/cryptic.json`

We provide a `main.py` script to help you get started. However, you can structure your code whichever way you think is best. We also provide a `scratchpad.ipynb` notebook to help you experiment with trying different solutions.

The crossword answers are included with the puzzles to help you validate your solutions, but your solution should complete the crossword without seeing any answers.

> **Note**: You can use any libraries or tools to build your solution. We also provide an OpenAI API if you prefer to use that.

## Setup Instructions

1. Clone this repository:
```bash
git clone https://github.com/ragntune/llm-crossword.git
cd llm-crossword
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up your environment variables:
```bash
cp .env.example .env #Copy the example env
# Edit the .env and replace with the values provided during the interview
```

5. Verify setup:

Run the main script:
```bash
python main.py
```

Or run the notebook cells in scratchpad.ipynb:

6. Start coding!

## Project Structure

```
llm_crossword/
├── src/                 # Source code
├── tests/              # Test suite
└── data/               # Data files
```

## Testing

Run the test suite:
```bash
pytest
```