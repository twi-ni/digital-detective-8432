# Mission 3 — Understand the operating system

## 1. Task
Explore how an operating system works, how it manages different parts of a computer, and understand things like running programs, storage, files and permissions. Document everything while making sure no personal information is shared.

## 2. Work completed
Completed Tasks 3.1 to 3.4 in `mission-3-task.md`:

- Task 3.1: Checked my macOS details, current user, available storage and running processes using Terminal commands.
- Task 3.2: Learned what processes and PIDs are and looked at examples of applications and background processes.
- Task 3.3: Understood the difference between absolute and relative paths and checked file permissions using Terminal.
- Task 3.4: Went through six main responsibilities of an operating system and understood them with everyday examples.

## 3. Commands / tools used

- `sw_vers`, `uname -m` — Checked my macOS version and processor details.
- `whoami` — Checked which user account I was logged into.
- `df -h /` — Checked how much storage was used and how much was available.
- `ps aux | head -n 10` — Viewed some of the processes running on my computer.
- `pwd`, `cd`, `ls -l` — Used these to move between folders, check file locations and view file permissions.
- Git (`git status`, `git add`, `git commit`, `git push`) — Used Git to save my work and upload the changes to GitHub.

## 4. My understanding

I understood that the operating system basically connects the hardware and the applications we use. It manages things like running programs, memory, storage and file permissions. I also learned that every running process gets its own PID, which helps the OS identify it. Overall, the OS makes sure everything works together properly, even when we're doing multiple things at once.

## 5. Difficulties faced

One thing I had to be careful about was not accidentally sharing personal information like my Mac username or the full location of my folders while documenting the commands and their outputs.

## 6. How I resolved them

I replaced personal details like my username and device information with `[redacted]` wherever needed. This helped me keep the documentation useful without exposing private information.

## 7. Evidence/files

- `mission-03-operating-system/mission-3-task.md` — Contains my completed answers and observations for Tasks 3.1 to 3.4.
- `mission-03-operating-system/README.md` — Contains the documentation for this mission.

## 8. Commit details

- Commit message: `Document operating system and file management`
- Push status: Successfully committed and pushed my Mission 3 folder to the `main` branch on GitHub.
