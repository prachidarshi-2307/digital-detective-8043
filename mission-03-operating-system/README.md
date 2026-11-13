# Mission 3: Operating Systems

## 1. Task / Objective

The objective of this mission was to explore the operating system, inspect running processes, understand file paths and permissions, and learn about the major responsibilities of an operating system.

I performed these activities on macOS using Terminal and explored how the operating system manages processes, storage, memory, files, and hardware resources.

## 2. Work Completed

### Task 3.1 — Exploring the Operating System

I used Terminal commands to inspect my operating system version, current account, available disk storage, and running system activity.

| Information explored | What it tells me | My observation |
|---|---|---|
| Operating system | Identifies the installed operating system and its version. | macOS, version 27.2, build 26B123. |
| Current account | Identifies the account currently logged into the system. | The command displayed my current username. I have kept this information private. |
| Available storage | Displays total, used, and available disk space. | 926 GiB total, 117 GiB used, 784 GiB available, with 13% capacity used. |
| System activity | Provides information about running processes, CPU usage, memory usage, and system load. | The snapshot showed 792 processes: 4 running and 788 sleeping. CPU usage was 8.46% user, 8.90% system, and 82.62% idle. |

### Task 3.2 — Understanding Processes

A process is an instance of a program that is currently running on a computer. Every process receives a unique Process ID (PID), which helps the operating system identify and manage it.

I used the command `ps aux | head -10` to view a snapshot of the running processes on my Mac.

**What does the PID column represent?**

PID stands for Process ID. It is a unique numerical identifier assigned to each running process by the operating system.

**Two examples of processes I observed:**

1. Google Chrome Helper (Renderer) — a process responsible for rendering and displaying browser content.
2. WindowServer — a macOS system process responsible for managing graphical windows and displaying content on the screen.

I also observed other processes, such as Chrome's video capture and audio services. This helped me understand that one application can create multiple processes to handle different tasks.

### Task 3.3 — Understanding Paths and Permissions

I used the `pwd` command to identify my current working directory and the `cd` command to navigate into the Mission 3 directory.

**Absolute path:**

An absolute path specifies the complete location of a file or directory, starting from the root directory.

Example:

`/Users/[redacted]/Desktop/digital-detective-8043/mission-03-operating-system`

**Relative path:**

A relative path specifies the location of a file or directory in relation to the current working directory.

Example:

`mission-03-operating-system`

This relative path can be used from the repository's root directory to access the Mission 3 folder.

I also used the following command to inspect the permissions of a file created during Mission 2:

`ls -l ../terminal-practice/notes.txt`

The output showed the permission string:

`-rw-r--r--`

**Understanding the permissions:**

- `-` indicates that the item is a regular file.
- `rw-` means the owner can read and write the file but cannot execute it.
- `r--` means group members can only read the file.
- `r--` means other users can only read the file.

This helped me understand how an operating system controls access to files through permissions.

### Task 3.4 — Responsibilities of an Operating System

| Responsibility | Explanation | Example |
|---|---|---|
| Process management | Manages running programs and distributes CPU time among them. | Managing Google Chrome and its multiple helper processes. |
| Memory management | Allocates and manages RAM for different applications and processes. | Providing memory to Google Chrome while it is running. |
| Device management | Coordinates communication between the operating system and hardware devices. | Managing the camera, audio devices, and display through system services. |
| File management | Organises files and directories and controls how they are stored and accessed. | Creating, saving, copying, and opening files in the assignment repository. |
| User interface / shell | Provides ways for users to interact with the computer through graphical interfaces or command-line tools. | Using the macOS desktop and Terminal. |
| Security and permissions | Controls access to files and system resources to protect data. | Using file permissions to decide who can read or modify `notes.txt`. |

## 3. Commands / Tools Used

The following commands were used during this mission:

| Command | Purpose |
|---|---|
| `sw_vers` | Displays macOS version information. |
| `whoami` | Displays the current account username. |
| `df -h .` | Displays disk storage information in a human-readable format. |
| `top -l 1 -n 5` | Displays a snapshot of system activity and processes. |
| `ps aux \| head -10` | Displays the first ten lines of the running process list. |
| `pwd` | Displays the current working directory. |
| `cd mission-03-operating-system` | Navigates into the Mission 3 directory. |
| `ls -l ../terminal-practice/notes.txt` | Displays detailed file information, including permissions. |

**Tools used:** macOS, Terminal, and Visual Studio Code.

## 4. My Understanding

Through this mission, I understood that an operating system acts as an interface between users, applications, and computer hardware.

I learned how to check system information, observe running processes, identify processes using their PIDs, navigate through directories using absolute and relative paths, and interpret file permissions.

I also understood that the operating system manages important resources such as CPU time, RAM, storage, and connected devices while providing a secure environment for applications to run.

## 5. Difficulties Faced

Initially, I found it slightly confusing to distinguish between absolute and relative paths. Understanding the different groups of file permissions and interpreting the process list were also new concepts for me.

## 6. How I Resolved Them

I practised navigating between the repository root and the Mission 3 directory using `pwd` and `cd`.

I inspected an existing practice file using `ls -l` and studied its permission string character by character. I also used `ps aux | head -10` to observe actual application and system processes.

These practical exercises helped me understand the concepts more clearly.

## 7. Evidence / Files

- Mission 3 README documenting the tasks and observations.
- Terminal commands and their outputs used to inspect macOS version, disk storage, system activity, and running processes.
- Directory navigation using `pwd` and `cd`.
- Permission inspection of `terminal-practice/notes.txt` using `ls -l`.

Personal account details, usernames, device names, and identifying file paths have been redacted from the documentation.

## 8. Commit Details

- Commit message: `Document operating system and file management`
- Changes pushed to the GitHub repository after completing Mission 3.