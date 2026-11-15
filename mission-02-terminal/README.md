# Mission 02 - Become comfortable with the Terminal

## 1. Task / objective

AI-assisted activity record: practise Terminal navigation, safe file operations, options, pipes, and package-manager inspection. Commands below were run in this repository; repeat them yourself and rewrite the explanations to meet the individual-work requirement.

## 2. Work completed

Created `terminal-practice/original.txt`, added two lines, copied it to `backup.txt`, renamed that copy to `backup-renamed.txt`, and displayed the contents. The displayed text contained both lines. A directory listing showed the original and renamed copy. The detailed listing included hidden entries and file sizes. Homebrew was already installed; no packages were changed.

### Command reference

| Operation | Command | What it does / observed |
|---|---|---|
| Current directory | `pwd` | Prints the full current path. The username was redacted from the saved record. |
| Directory listing | `ls` | Shows names in the current folder. |
| Detailed listing | `ls -lA` | Shows details and hidden entries; `-l` is long format and `-A` includes hidden names except `.` and `..`. |
| Parent directory | `cd ..` | Moves the shell's current location one directory up. |
| Create folder | `mkdir terminal-practice` | Creates a directory for the exercise. |
| Create empty file | `touch original.txt` | Creates an empty file or updates an existing file's timestamp. |
| Write / replace | `printf 'First line\n' > original.txt` | `>` replaces the file contents with the new output. |
| Append | `printf 'Second line\n' >> original.txt` | `>>` adds output at the end; both lines remained. |
| Copy | `cp original.txt backup.txt` | Makes a second file while keeping the original. |
| Move / rename | `mv backup.txt backup-renamed.txt` | Changes the path/name of the copy. |
| Display contents | `cat original.txt` | Printed both saved lines. |
| Flags and readable sizes | `ls -lah` | `-a` includes hidden entries, `-h` makes sizes easier to read, and `-l` shows details. |
| Pipe | `ls -lA | head -n 5` | The pipe passes the listing to `head`, which showed only the first five lines. |

Homebrew check: `brew --version` reported Homebrew 7.0.8. `brew list` showed the existing packages; nothing was installed or removed.

## 3. Commands / tools used

`pwd`, `ls`, `ls -lA`, `cd ..`, `mkdir`, `touch`, `printf`, `cp`, `mv`, `cat`, `head`, `brew --version`, and `brew list`.

## 4. My understanding

Reference note: `>` replaces a file's contents; `>>` appends. Copying creates another file, while moving or renaming changes the original file's location or name. `pwd` gives context for relative paths; `ls` helps inspect what is present. A pipe connects one command's output to another command's input. Rewrite these points in your own words.

## 5. Difficulties faced

No command failed in this practice. The detailed listing included the account name, so it was redacted from the saved record.

## 6. How I resolved them

Used a redacted listing in the notes and kept all file changes inside `terminal-practice/`.

## 7. Evidence / files

`terminal-practice/original.txt` and `terminal-practice/backup-renamed.txt` contain the two practice lines. Listing outputs were inspected but not saved because they include local account information.

## 8. Commit details

Commit message: `Complete Terminal and file management mission`. The explanations still need learner review and rewording.
