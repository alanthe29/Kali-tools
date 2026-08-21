# 🎓 Bash Learning - Day 1

## What is this?

This is my learning notebook for **Bash** (a programming language for computers). I'm documenting everything I learn step-by-step.

---

## Why did I make it?

To keep track of my learning journey and understand how to write **Bash scripts** (small programs written in Bash).

---

## What will I learn?

✅ How to write Bash code  
✅ How to run Bash programs  
✅ Basic computer science concepts  
✅ How to use Kali Linux commands  

---

## What is Bash?

**Bash** = A simple programming language that lets you talk to your computer by typing commands.

Think of it like giving instructions to your computer in a special language it understands.

---

## What do I need before starting?

**Prerequisites** (things you need already) = 

- A computer with Linux or Kali Linux (a special Linux version for hacking tools)
- A text editor (a program to write code) like Notepad or VSCode
- That's it! Just basic computer knowledge

---

## How do I run the code?

Follow these 3 simple steps:

### Step 1: Make the file runnable

```bash
chmod +x scripts/hello.sh
```

**What does this mean?**
- `chmod` = "change mode" (give permission)
- `+x` = "add execute permission" (let the computer run this file)
- `scripts/hello.sh` = the name of the file we want to run

### Step 2: Run the program

```bash
./scripts/hello.sh
```

**What does this mean?**
- `./` = "run this file from the current folder"
- `scripts/hello.sh` = the file name

### Step 3: See the result

Your computer will print:
```
Hello, World!
```

---

## Folder structure (where files are)

```
Kali-tools/
│
├── README.md          ← This file (you are here!)
│
└── scripts/           ← Folder with Bash programs
    └── hello.sh       ← Our first program
```

---

## What is a `.sh` file?

`.sh` = A file that contains Bash code (just like `.txt` is a text file, `.sh` is a Bash file)

---

## Common mistakes & how to fix them

### ❌ Error: "Permission denied"

**Problem:** When you run `./scripts/hello.sh`, it says "Permission denied"

**Fix:** You forgot to make it runnable. Do this:
```bash
chmod +x scripts/hello.sh
```

Then try again:
```bash
./scripts/hello.sh
```

---

### ❌ Error: "No such file or directory"

**Problem:** It can't find the file

**Fix:** Make sure you're in the correct folder:
```bash
# Check where you are
pwd

# You should see: /path/to/Kali-tools
```

If you're not there, go there:
```bash
cd Kali-tools
```

Then run:
```bash
./scripts/hello.sh
```

---

### ❌ Error: "bash: ./scripts/hello.sh: command not found"

**Problem:** The file doesn't exist yet

**Fix:** Make sure `hello.sh` is in the `scripts` folder. You can check with:
```bash
ls scripts/
```

You should see `hello.sh` in the list.

---

## Simple Bash commands to know

### See what's in a folder

```bash
ls
```

This shows all files and folders in the current location.

---

### Go to a folder

```bash
cd scripts
```

This takes you into the `scripts` folder.

---

### Go back up

```bash
cd ..
```

This takes you to the parent folder (one level up).

---

### Check where you are

```bash
pwd
```

This shows your current location.

---

### Read a file

```bash
cat hello.sh
```

This shows what's inside the `hello.sh` file.

---

## Inside `hello.sh` - What does the code mean?

```bash
#!/bin/bash
echo "Hello, World!"
```

Let me break this down:

**Line 1:** `#!/bin/bash`
- `#!` = "Hey computer, this is special"
- `/bin/bash` = "Use Bash to run this file"
- (This must be the first line of every Bash file!)

**Line 2:** `echo "Hello, World!"`
- `echo` = "Print this on the screen"
- `"Hello, World!"` = The text to print
- So this line prints: `Hello, World!`

---

## Next steps (what to do after Day 1)

When you're comfortable with this, you can learn:

- **Day 2:** Variables (storing information)
- **Day 3:** Loops (doing things many times)
- **Day 4:** If statements (making decisions)
- **Day 5:** Functions (organizing your code)

---

## Helpful links (if you get stuck)

- [Bash basics guide](https://www.gnu.org/software/bash/manual/bash.html) (official instructions)
- [Linux commands guide](https://www.linux.com/training-tutorials/linux-101-introduction-linux/) (learn more about Linux)
- [Kali Linux guide](https://www.kali.org/) (learn about Kali Linux)

---

## Questions?

If something doesn't work or you don't understand:

1. Read the error message carefully
2. Check the "Common mistakes" section above
3. Try again with the fix

---

**Keep learning! You got this! 🚀**

---

*Started: Day 1 - 2026-08-21*
