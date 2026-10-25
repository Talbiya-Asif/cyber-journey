# Linux Notes - Bandit 0-10 and TryHackMe Part 1
Date: 2026-10-24

## What I did
- Finished TryHackMe Linux Fundamentals Part 1
- Completed OverTheWire Bandit levels 0 to 10 (SSH from PowerShell)
- Completed Google Cybersecurity Cert, Course 1, Module 1 (94%)

## Commands I learned
- whoami : shows which user I am
- echo : prints text to the screen
- ls : lists files in a folder
- ls -a : lists ALL files, including hidden ones (names start with a dot)
- cd : moves into a folder
- pwd : shows the folder I am in
- cat : prints what is inside a file
- find : searches for files by type, size, owner
    find . -type f -size 1033c
- grep : prints the lines of a file that contain a word
    grep millionth data.txt
- sort : puts lines in order, so identical lines sit together
- uniq -u : prints only lines that appear once (needs sorted input)
    sort data.txt | uniq -u
- strings : pulls readable text out of a binary file
- file : tells me a file's type (text or data)
    file ./*
- base64 -d : decodes base64 text
- ssh : connects to another computer

## Symbols and tricks
- Pipe | : sends the output of one command into the next
- > : sends output into a file and overwrites it
- >> : adds output to the end of a file without overwriting
- ./ before a file name : stops names starting with - being read as options (cat ./-)
- Quotes : keep a file name with spaces as one name
- Asterisk * : matches many files at once
- 2>/dev/null : hides error messages
- Tab key : finishes a file name for me

## What I understood
- Hidden files start with a dot, so ls skips them and ls -a shows them
- In -size 1033c, the c means bytes
- grep prints the whole line that contains the word (like Ctrl+F)
- uniq only compares neighbouring lines, so sort comes first
- strings shows human-readable text inside binary data

## Mistakes I made and fixed
- Wrong hostname gave "No such host"
- Used bandit0 with the Level 1 password (each level has its own username)
- Copied the whole ls -a output instead of one file name
- cat on a binary file printed garbage; use file ./* first

## What confused me
- The new commands were a bit overwhelming but as i used them they got easier i was confused by hidden files, multiple files and how to change or add to commands to use it but than it got easier as i read the function of each command

## Rules
- Never post Bandit passwords or solutions online
- Keep passwords in a private note on my laptop only, never on GitHub 