# Mission 3 — Understand the operating system

## Task 3.1 — Explore your operating system

| Information explored | What it tells you | Your observation (privacy-safe) |
| --- | --- | --- |
| Operating system/system details | Shows which operating system the computer is running, its version and processor architecture. | My system runs macOS. I checked this using `sw_vers` and `uname -m`. |
| Current account identity | Shows the username of the account currently logged into the computer. | The username was redacted, but it confirmed that I was logged in through a regular local user account and not as `root`. |
| Available and used storage | Shows how much storage is being used and how much space is still available. | I checked the main `/` volume and could see the total storage, used space and remaining space in GB. |
| System activity snapshot | Shows the programs and processes currently running along with their CPU and memory usage. | I used `ps aux | head -n 10` and saw different macOS background services and Terminal processes running. |

---

## Task 3.2 — Understand processes

* What is a process?  
  A process is basically a program that is currently running on a computer. For example, whenever I open an application, it starts running as a process and uses system resources like RAM and CPU.

* What does the PID column represent?  
  PID stands for Process ID. It is a unique number given to every running process so the operating system can identify and manage it separately.

* Two examples of processes that may be running on your computer:
  1. Application process: Google Chrome or VS Code running while I am working.
  2. Background system process: `WindowServer` or `Finder`, which helps manage the desktop and things displayed on the screen.

---

## Task 3.3 — Understand paths and permissions

* Difference between an absolute path and a relative path:

  * Absolute path: Gives the complete location of a file starting from the root directory. It stays the same no matter which folder I am currently working in.
    * Example: `/Users/[redacted]/Desktop/digital-detective-8432/terminal-practice`

  * Relative path: Gives the location of a file based on the folder I am currently in, without having to type the entire path.
    * Example: `terminal-practice/notes.txt` (when run from inside the main assignment folder).

* Owner permissions check (`ls -l`):

  When I checked `terminal-practice/notes.txt` using `ls -l`, I got the permissions as `-rw-r--r--`. This means that I can read and edit the file as its owner, but I cannot execute it. Other users can only read the file.

---

## Task 3.4 — Explain operating-system responsibilities

| OS responsibility | Your explanation | Example |
| --- | --- | --- |
| Process management | The OS manages all the programs running at the same time and decides how much CPU time each program gets. | Running VS Code, Chrome and Terminal together without having to close one to use another. |
| Memory management | It keeps track of how much RAM different applications are using and manages memory when programs are opened or closed. | Giving memory to open browser tabs and freeing it when I close them. |
| Device management | It helps the operating system communicate with hardware devices so they work properly. | Registering keyboard presses and trackpad clicks and showing the results on the screen. |
| File management | It takes care of storing and organizing files and folders so we can easily find and access them. | Creating, saving, renaming and organizing my assignment folders in Finder. |
| User interface/shell | It provides the ways through which we interact with the computer, either by clicking things or entering commands. | Using the macOS desktop or typing commands in Terminal. |
| Security and permissions | It protects files and system settings by deciding which users can access, edit or make changes to them. | Asking for a password before allowing certain system-level changes. |