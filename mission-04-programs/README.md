# Mission 04 - How programs run

## 1. Task / objective

AI-assisted draft: create and run `hello.py`, then compare compiler and interpreter approaches. The script was run in the local assignment folder; review and explain the result in your own words.

## 2. Work completed

Created `hello.py` containing `print("Hello from Python")` and ran it. The Terminal displayed `Hello from Python`.

| Point | Compiler | Interpreter |
|---|---|---|
| When execution/translation happens | Usually translates source before running the program. | Executes instructions during program runtime. |
| Typical output | A translated program, often machine code or another intermediate form. | Program actions/results produced as it reads and executes instructions. |
| Example | C compiler such as Clang. | Python runtime (Python also compiles source to bytecode internally). |
| Advantage | Compiled output can run quickly without translating source on each start. | Quick to try and change code; errors can be tied to the statement being executed. |

Short comparison draft: A compiler translates program source before execution, while an interpreter carries out program instructions at runtime. Compiled programs often produce a separate executable or intermediate file. Interpreted workflows make small experiments easy. Real language implementations can mix these approaches, as Python does with bytecode.

## 3. Commands / tools used

`python3 hello.py` ran the program with Python 3. The installed version is Python 3.9.6.

## 4. My understanding

Reference note: the important distinction is when translation and execution happen. Many real language implementations combine compilation and interpretation. Rephrase the short comparison above after understanding it.

## 5. Difficulties faced

No error occurred; the output matched the one-line program.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

`hello.py`.

## 8. Commit details

Commit message: `Compare compilers and interpreters`.
