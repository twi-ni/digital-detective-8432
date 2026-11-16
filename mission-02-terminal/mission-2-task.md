
# Mission 2 - Become Comfortable with the Terminal

## Task 2.1 - Explore basic Terminal operations

| Command | What it does | What I observed |
| --- | --- | --- |
| `pwd` | Shows the folder I am currently in. | It showed the full path to my repository folder. |
| `ls` | Shows the files and folders in the current folder. | I could see all my mission folders and the README file. |
| `ls -l` | Shows the files with more details like size and permissions. | Each file was shown on a separate line with its details. |
| `cd ..` | Takes me one folder back. | I used `pwd` again and saw that I had moved to the parent folder. |
| `mkdir` | Creates a new folder. | My new practice folder was created successfully. |
| `touch` | Creates an empty file. | It created a blank text file with 0 bytes. |
| `cp` | Copies a file. | I could see both the original file and its copy. |
| `mv` | Moves or renames a file. | The old filename changed to the new one. |
| `cat` | Shows what's written inside a file. | The text appeared directly in the Terminal. |

## Task 2.2 - Practise file changes safely

1. What is the difference between replacing a file's contents and adding text to the end?
When I use `>`, the old content gets replaced with the new text. But `>>` adds the new text at the end without removing what was already there.

2. What is the difference between copying a file and moving a file?
`cp` makes another copy of the file, so the original stays where it is. `mv` moves the file to another place or changes its name.

3. What information does the current directory display provide?
The `pwd` command tells me exactly which folder I am currently working in. This is useful because I know where the files I create or change will be.

4. Why is a directory-listing operation useful?
Commands like `ls` help me see what files and folders are present. I can also use `ls -l` to check more details and make sure my files were created or renamed properly.

## Task 2.3 - Understand flags and pipes

1. Normal listing (`ls`) vs detailed listing (`ls -lah`)
`ls` just shows the file and folder names. When I use `ls -lah`, I get more information like file sizes, permissions and dates. It also shows hidden files, such as `.git`, which normally don't appear in a regular listing.

2. Pipe example (`ls -l | head -n 5`) and how it works
The `|` symbol is called a pipe. It takes the output of one command and sends it to the next command.
- `ls -l` shows the detailed list of files and folders.
- `head -n 5` displays only the first 5 lines from that list.
So instead of seeing the entire list, I only get the first five lines.

## Task 2.4 - Understand package managers

A package manager helps us install, update and remove software without having to download and set up everything manually. On macOS, one example is Homebrew, which is also called `brew`. It can be used to install different tools and applications directly through the Terminal.
