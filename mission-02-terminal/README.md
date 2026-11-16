# Mission 2 — Become comfortable with the Terminal

## 1. Task 
Learn to navigate directories, manage files safely, use command-line flags and pipes, and understand how package managers work on macOS.

## 2. Work completed
Completed all four tasks for Mission 2 in `mission-2-task.md` and practised commands inside `terminal-practice/`:
- Task 2.1: Performed basic terminal operations and recorded observations in a reference table.
- Task 2.2: Created a text file inside `terminal-practice/`, wrote and appended lines safely, created a backup copy and answered file-safety questions.
- Task 2.3: Compared `ls` with `ls -lah` and used a pipe to limit output lines.
- Task 2.4: Checked Homebrew status safely without modifying system packages and documented how package managers work.

## 3. Commands/tools used
- `pwd`, `ls`, `ls -l`, `ls -lah`, `cd` — Directory navigation and detailed/hidden file inspection.
- `mkdir`, `touch`, `cp`, `mv`, `cat` — Creating, copying, renaming and reading files and folders.
- `echo`, `>`, `>>` — Writing and appending text to files.
- `|` and `head -n 5` — Chaining commands to filter output.
- `brew --version` — Checking whether Homebrew is installed on macOS.
- Git (`git status`, `git add`, `git commit`, `git push`) — Version control and publishing to GitHub.

## 4. My understanding
The terminal allows fast, precise control over files and folders without needing a graphical interface. Using `>>` instead of `>` prevents accidentally overwriting existing file data, while flags like `-lah` reveal hidden files and readable sizes. Pipes make the terminal modular by letting one command's output feed directly into another command's input and package managers like Homebrew simplify managing developer software safely.

## 5. Difficulties faced
Making sure terminal screenshots did not expose private username or device details.

## 6. How I resolved them
Cropped the prompt area out of screenshots before saving them to `evidence/`.

## 7. Evidence / files
- `mission-02-terminal/mission-2-task.md` — Completed command reference table and answers for Tasks 2.1–2.4.
- `terminal-practice/` — Practice folder containing created and backed-up text files.
- `mission-02-terminal/evidence/` — Privacy safe cropped screenshots of terminal operations.
- `mission-02-terminal/README.md` — Mission 2 documentation.

## 8. Commit details
- **Commit message:** `Complete Terminal and file management mission`
- **Push status:** Committed and pushed Mission 2 files and evidence to the `main` branch on GitHub.
