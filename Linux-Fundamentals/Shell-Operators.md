# Shell Operators

Shell operators allow you to combine commands, redirect output, and run commands more efficiently in Linux.

---

## &

**Purpose:** Runs a command in the background.

### Example

```bash
cp largefile.txt backup/ &
```

### Explanation

Runs the copy command in the background so you can continue using the terminal.

---

## &&

**Purpose:** Runs the next command only if the first command succeeds.

### Example

```bash
cd Documents && ls
```

### Explanation

Changes into the Documents folder and then lists its contents only if the `cd` command succeeds.

---

## >

**Purpose:** Redirects output to a file and overwrites the existing contents.

### Example

```bash
echo "password123" > passwords
```

### Explanation

Creates or overwrites the file `passwords` with the text `password123`.

---

## >>

**Purpose:** Appends output to the end of a file without overwriting existing content.

### Example

```bash
echo "tryhackme" >> passwords
```

### Explanation

Adds `tryhackme` to the end of the `passwords` file while keeping everything already inside the file.

---

# Notes

- `>` replaces the contents of a file.
- `>>` adds new content to the end of a file.
- `&&` is useful for running multiple commands in sequence.
- `&` runs a command in the background while you continue using the terminal.

---

# Real-World Examples

### Run a large file copy in the background

```bash
cp largefile.txt backup/ &
```

Useful when copying large files so you can continue working.

---

### Change folders and immediately list files

```bash
cd Documents && ls
```

Commonly used by Linux administrators to verify they entered the correct directory.

---

### Create or overwrite a configuration file

```bash
echo "password123" > passwords
```

Used when creating new files or replacing old contents.

---

### Append information to a log file

```bash
echo "tryhackme" >> passwords
```

Useful for adding new information without deleting previous data.

---

# Summary

Shell operators make Linux much more powerful by allowing you to:

- Run commands in the background
- Chain commands together
- Redirect output into files
- Append data without deleting existing information
