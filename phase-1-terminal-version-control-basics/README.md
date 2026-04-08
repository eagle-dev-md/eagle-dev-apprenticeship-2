# Phase 1: Terminal & Version Control Basics

Before diving into HTML and CSS, you need to get comfortable with the tools of the trade. This phase introduces you to the terminal and Git, which are essential for managing your code and collaborating with others.

## Concepts
- terminal commands
- Git basics
- repository management

## Micro Project
Create a GitHub repository for your future projects and practice pushing and pulling changes.
# Getting Comfortable with Terminal Commands

## Overview

Think of your terminal as the **backstage pass to your computer**. Just like a concert where you need a special pass to access the backstage area, terminal commands let you communicate directly with your computer, bypassing the flashy UI.

When you type a command, it's like giving your computer a specific instruction — akin to telling a band member exactly what song to play next.

---

## Basic Commands

| Command | What it does | Analogy |
|--------|--------------|---------|
| `cd` | Change directory | Moving from one part of the venue to another |
| `ls` | List files in a directory | Asking the stage manager "what's in the green room?" |
| `mkdir` | Create a new directory | Setting up a new merchandise booth |
| `touch` | Create a new file | Adding a new item to the booth |
| `rm` | Remove files or directories | Cleanup crew after the show |

---

## Navigating Directories

```bash
# Start in your home directory
cd ~

# Move into Documents
cd Documents

# See what's inside
ls

# Dive into a specific project
cd my-project

# Full detailed listing including hidden files
ls -la

# Go back up one level (now back in Documents)
cd ..

# List contents again to confirm where you are
ls

# Re-enter the project folder
cd my-project
```

### Key Insight

- `cd ..` moves you **one level up** only
- To jump straight to a known location from anywhere, use the **full path**:

```bash
cd ~/Documents/my-project
```

---

## Understanding `ls -la`

The `-la` flags mean:
- `-l` — long format (permissions, owner, size, date)
- `-a` — **all files**, including hidden ones (dot-prefixed)

### Example output:

```
total 64
drwxr-xr-x  6 user user 4096 Apr  8 10:00 .
drwxr-xr-x 20 user user 4096 Apr  7 09:00 ..
-rw-r--r--  1 user user  234 Apr  8 09:00 .env
drwxr-xr-x  8 user user 4096 Apr  8 10:00 .git
-rw-r--r--  1 user user   12 Apr  8 09:00 .gitignore
-rw-r--r--  1 user user  123 Apr  8 10:00 index.js
drwxr-xr-x  4 user user 4096 Apr  8 09:30 node_modules
-rw-r--r--  1 user user  890 Apr  8 09:30 package.json
-rw-r--r--  1 user user  567 Apr  8 09:30 package-lock.json
```

Hidden files in a Node.js project commonly include `.env`, `.gitignore`, `.git/`, `.eslintrc`, and `.prettierrc`.

---

## Today's Assignment

### Getting Comfortable with Terminal Commands

Work through each step below and confirm the expected output at each stage.

### Step 1 — Open terminal & navigate to a directory

```bash
cd ~/Documents
```

✅ You are now in your Documents folder.

### Step 2 — Create a new directory & confirm it

```bash
mkdir my-practice-folder
ls
```

✅ `ls` should show `my-practice-folder` in the list.

### Step 3 — Navigate into it & list files

```bash
cd my-practice-folder
ls
```

✅ It will be empty for now — that is expected.

### Step 4 — Create a new file & verify it

```bash
touch hello.txt
ls
```

✅ You should now see `hello.txt` listed.

### Step 5 — Delete the file & confirm deletion

```bash
rm hello.txt
ls
```

✅ `hello.txt` should no longer appear in the list.

---

## Full Sequence (Start to Finish)

```bash
cd ~/Documents
mkdir my-practice-folder
ls
cd my-practice-folder
ls
touch hello.txt
ls
rm hello.txt
ls
```

> 💡 **Tip:** Run each line one at a time and observe the output after each step.

---

## Acceptance Criteria

- [ ] You can open the terminal and navigate to a specific directory using `cd`
- [ ] You can create a new directory using `mkdir` and confirm its creation
- [ ] You can list files in a directory using `ls` and confirm it shows the expected output
- [ ] You can create a new file using `touch` and verify its existence with `ls`
- [ ] You can delete a file using `rm` and confirm its deletion
