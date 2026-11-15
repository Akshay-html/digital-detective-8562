# Mission 03 - Understand the operating system

## 1. Task / objective

AI-assisted draft: inspect system details, account, storage, processes, paths, file permissions, and core OS responsibilities. Personal names and paths are omitted or redacted from this public repository.

## 2. Work completed

### System observations

| Information | What it tells you | Privacy-safe observation |
|---|---|---|
| OS | The operating system manages hardware and applications. | macOS 26.6 (build 25G72). |
| Current account | Which account owns the active session. | `whoami` identifies the account; the name is intentionally not published. |
| Storage | How much space is used and available on the mounted volume. | At the time checked, `/` showed 460 GiB total, 12 GiB used, 360 GiB available (4% used). |
| Memory | Installed RAM and current memory use. | 16 GB physical memory; Activity Monitor reported about 11.7 GB used during the snapshot. |
| Processes | Programs currently running; each has a PID. | Activity Monitor was opened. Its process rows were not exposed in this restricted environment, so no process/PID sample is recorded. |

### Paths and permissions

- Absolute path example (username redacted): `/Users/[redacted]/.../digital-detective-8562/mission-03-operating-system/README.md`.
- Relative path from the repository root: `mission-03-operating-system/README.md`.
- The practice file permission mode was `-rw-r--r--`: its owner can read and write it, but it is not executable.
- A process is a running program. A PID is the number the operating system uses to identify a particular process. Finder and Activity Monitor were open; their PIDs still need to be read from the process list.

### Operating-system responsibilities

| Responsibility | Short explanation | Example |
|---|---|---|
| Process management | Starts and schedules running programs. | Keeps a browser and editor running. |
| Memory management | Gives programs working memory and reclaims it when possible. | Allocates memory to an open document. |
| Device management | Coordinates access to hardware. | Sends keyboard input to the active app. |
| File management | Organises files and storage locations. | Saves a note into a folder. |
| User interface / shell | Lets a person control the computer. | Finder windows or Terminal commands. |
| Security / permissions | Controls who may read, change, or run files. | A file's read/write/execute permissions. |

## 3. Commands / tools used

`sw_vers`, `df -h /`, `whoami` (account name not published), `stat -f '%Sp %N'`, and Activity Monitor. `top` and `ps` were blocked by the restricted environment.

## 4. My understanding

Reference note: a process is one running instance of a program; its PID distinguishes it from other processes. An absolute path starts at the filesystem root; a relative path is interpreted from the current directory. Read, write, and execute permissions describe whether an account can view, change, or run a file. Rewrite these notes in your own words.

## 5. Difficulties faced

The shell returned “operation not permitted” for process-list commands, and Activity Monitor showed column headings but no readable process rows in this restricted session.

## 6. How I resolved them

System version, storage, and file permissions were gathered with permitted read-only commands. Process names and PIDs remain unverified and must be captured directly in Activity Monitor on the learner's computer.

## 7. Evidence / files

`mission-02-terminal/terminal-practice/original.txt` was used to inspect permissions. This README contains redacted system observations; no screenshot with account, device, or network identifiers is included.

## 8. Commit details

Commit message: `Document operating system and file management`. Mission remains incomplete until the learner records real process names/PIDs and reviews the notes.
