
# Mission 3 - Understand the Operating System

## Task 3.1 - Explore your operating system

| Information explored | What it tells you | What I observed |
| --- | --- | --- |
| Operating system/system details | Shows which OS the computer is using, its version and processor type. | My computer runs macOS. I checked it using `sw_vers` and `uname -m`. |
| Current account identity | Shows which user account is currently logged in. | I hid my username for privacy, but I could confirm that I was using a normal local account and not the `root` account. |
| Available and used storage | Shows how much storage is already used and how much is still free. | I checked the main `/` volume and saw the total, used and available storage in GB. |
| System activity snapshot | Shows which programs are running and how much CPU and memory they are using. | I used `ps aux | head -n 10` and saw different macOS background processes and Terminal processes. |

---

## Task 3.2 - Understand processes

1. What is a process?
A process is just a program that is running on the computer. For example, when I open Chrome or VS Code, it starts running as a process and uses things like RAM and CPU.

2. What does the PID column represent?
PID means Process ID. Every running process gets its own number so the operating system can identify it and keep track of it.

3. Two examples of processes that may be running on your computer:
1. Application process: Google Chrome or VS Code when I am using them.
2. Background system process: `WindowServer` or `Finder`, which help manage the desktop and what appears on the screen.

---

## Task 3.3 - Understand paths and permissions

1. What is the difference between an absolute path and a relative path?
- Absolute path: It gives the full location of a file starting from the root folder. It doesn't depend on which folder I am currently in.
  Example: `/Users/[redacted]/Desktop/digital-detective-8432/terminal-practice`

- Relative path: It gives the file location based on the folder I am already working in, so I don't have to type the full path.
  Example: `terminal-practice/notes.txt` (when I am inside the main assignment folder).

2. Owner permissions check (`ls -l`):
I checked `terminal-practice/notes.txt` using `ls -l` and got `-rw-r--r--` as the permission value. This means I can read and edit the file because I am its owner. Other users can only read it, and nobody has permission to execute it.

---

## Task 3.4 - Explain operating system responsibilities

| OS responsibility | My explanation | Example |
| --- | --- | --- |
| Process management | The OS manages the programs running on the computer and decides how they share the CPU. | Using VS Code, Chrome and Terminal at the same time. |
| Memory management | It keeps track of the RAM being used by different applications. | Giving memory to browser tabs and managing it when I close them. |
| Device management | It helps the computer communicate with connected hardware devices. | Detecting keyboard presses and trackpad clicks. |
| File management | It helps store and organise files and folders so they are easier to find. | Creating, saving and renaming my assignment folders in Finder. |
| User interface/shell | It gives us a way to interact with the computer, either through the screen or by typing commands. | Using the macOS desktop and Terminal. |
| Security and permissions | It controls who can access or make changes to files and system settings. | Asking for a password before allowing certain system changes. |
