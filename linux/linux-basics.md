🐧 Linux Fundamentals

1. Linux Basics

- Linux is an open-source operating system.
- Kali Linux is a Debian-based Linux distribution used for cybersecurity and penetration testing.
- The terminal allows us to interact with Linux using commands.

2. Basic Navigation Commands

Command        | Purpose
"pwd"          | Shows current directory
"ls"           | Lists files and directories
"ls -a"        | Shows hidden files
"ls -l"        | Shows detailed file information
"cd directory" | Enters a directory
"cd .."        | Moves to parent directory
"cd ~"         | Moves to home directory

3. File and Directory Commands

Command          | Purpose
"mkdir test"     | Creates a directory
"touch file.txt" | Creates an empty file
"cp a.txt b.txt" | Copies a file
"mv a.txt b.txt" | Moves or renames a file
"rm file.txt"    | Deletes a file
"rmdir test"     | Removes an empty directory

4. Reading Files

Command               | Purpose
"cat file.txt"        | Displays file contents
"less file.txt"       | Views a file page by page
"head -n 5 file.txt"  | Shows first 5 lines
"tail -n 5 file.txt"  | Shows last 5 lines
"wc -l file.txt"      | Counts lines

5. Searching

- "grep \"text\" file.txt" — searches for text.
- "grep -i \"text\" file.txt" — ignores case.
- "grep -n \"text\" file.txt" — displays matching line numbers.
- "find ~ -type f -name \"*.txt\"" — finds text files in the home directory.

6. Linux Permissions

Linux permissions:

- "r" = Read (4)
- "w" = Write (2)
- "x" = Execute (1)

Examples:

- "chmod 600 file.txt" — owner can read and write.
- "chmod 644 file.txt" — owner can read/write; others can read.
- "chmod 755 script.sh" — owner has full permissions; others can read/execute.

Important commands:

- "ls -l" — checks permissions.
- "chmod" — changes permissions.
- "sudo" — runs a command with elevated privileges.

7. Processes and Services

- "ps" — displays processes.
- "ps aux" — displays detailed process information.
- "top" — monitors running processes.
- "free -h" — displays memory usage.
- "systemctl status NetworkManager" — checks NetworkManager service status.

Key Takeaway

Linux fundamentals are essential for cybersecurity because security tools, scripts, services, files, and system processes are managed through the operating system.
