# Day 5: Starting the Cybersecurity Lab

## Theme

Today we stop only talking about the lab and actually start using it.

Day 5 is about taking the learning space we designed on Day 4 and turning it into something real.

This is not about hacking anything.

This is not about doing advanced cybersecurity.

This is about opening a safe practice environment and proving to yourself:

> I can build a lab.  
> I can use Linux.  
> I can practice cybersecurity without breaking my real computer.

---

## Core Goal

By the end of today, the learner should understand:

- What a virtual machine is
- Why cybersecurity labs use virtual machines
- How a virtual machine protects the real computer
- What it means to practice safely
- How to open the lab environment for the first time
- How to document proof that the lab is working

---

## Plain-English Explanation

A cybersecurity lab is just a safe place to practice.

Think of it like a workshop.

If you wanted to learn how to fix engines, you would not start by tearing apart the only car you need to get to work.

You would practice on something separate.

That is what a virtual machine does.

A virtual machine is like a computer inside your computer. It acts like a separate machine, but it runs inside a program.

That means you can practice Linux, networking, commands, and cybersecurity basics without putting your main computer at risk.

You are not trying to become an expert today.

You are proving that the lab can open, run, and be used safely.

---

## What We Are Building Today

Today we are starting the first working part of the REBUILD45 home cybersecurity lab.

The lab will be simple:

```text
Real Computer
│
└── Virtualization Software
    │
    └── Linux Virtual Machine
```

That Linux virtual machine becomes the practice computer.

It is where we can make mistakes, learn commands, test tools, and build confidence.

---

## Important Mindset

A lot of adults get stuck here because they think:

> I should already know this.

No.

You should not already know this.

That is the whole point of building the lab.

The lab exists so you can learn safely.

Today is not about being fast.

Today is about getting one working environment opened and documented.

---

## Step 1: Open Your Virtualization Software

Open the virtualization program you chose on Day 4.

Common examples include:

- VirtualBox
- VMware Workstation Player
- UTM
- Hyper-V
- Parallels

Do not worry if yours looks different from someone else’s.

The goal is simple:

Open the program and confirm that you can see where virtual machines are created or listed.

---

## Step 2: Start or Create the Linux Virtual Machine

If you already created a Linux virtual machine, start it.

If you have not created one yet, today is the day to begin setting it up.

The beginner-friendly choice is usually:

```text
Ubuntu Desktop
```

Ubuntu is a good starting point because it is common, well-documented, and easier for beginners to understand than many other Linux versions.

For this project, we are not trying to impress advanced Linux users.

We are trying to build confidence.

---

## Step 3: Understand What Is Happening

When the Linux virtual machine starts, your computer is running another computer inside a window.

That may sound strange at first, but it is one of the most important ideas in cybersecurity learning.

You now have a safe practice machine.

You can use it to:

- Learn Linux commands
- Practice networking basics
- Test cybersecurity tools
- Take screenshots for documentation
- Make mistakes without damaging your main computer

This is where real learning starts.

---

## Step 4: Log In and Look Around

Once the Linux virtual machine opens, do not rush.

Look around.

Notice the desktop.

Notice the menu.

Notice the file manager.

Notice the terminal.

This is your lab environment.

You do not need to understand everything yet.

Today you are simply becoming familiar with the space.

A good first win is opening the terminal.

The terminal is where many Linux and cybersecurity tasks happen.

Open it and type:

```bash
whoami
```

Then press Enter.

This command tells you the current user account.

You may see something like:

```bash
student
```

or:

```bash
rebuild45
```

or whatever username you created.

That tiny command matters.

You just interacted with Linux through the command line.

That is a real step.

---

## Step 5: Run the First Lab Check

Now type:

```bash
pwd
```

This means:

```text
print working directory
```

In plain English, it shows where you are currently located inside the file system.

You may see something like:

```bash
/home/yourname
```

That means you are inside your user’s home folder.

Now type:

```bash
ls
```

This lists the files and folders in the current location.

You may see folders like:

```bash
Desktop
Documents
Downloads
Pictures
```

These commands are basic, but they are not pointless.

They are the foundation of using Linux.

Cybersecurity tools are often built on top of simple commands like this.

---

## First Commands Used Today

```bash
whoami
pwd
ls
```

### What They Mean

| Command | Plain-English Meaning |
|---|---|
| `whoami` | Shows which user you are logged in as |
| `pwd` | Shows where you are in the file system |
| `ls` | Lists files and folders in the current location |

---

## Beginner Safety Note

Do not run random commands from the internet.

Do not copy and paste commands you do not understand yet.

Do not install cybersecurity tools just because someone online says they are cool.

The REBUILD45 lab is going to build slowly and safely.

The goal is understanding, not chaos.

---

## What To Document Today

Create a short Day 5 note with:

````markdown
# Day 5 Lab Notes

## What I Did

Today I opened my virtualization software and started my Linux virtual machine.

## What I Learned

A virtual machine is a safe practice computer inside my real computer.

## Commands I Used

```bash
whoami
pwd
ls
```

## What I Understand Now

I understand that the lab gives me a safe place to practice Linux and cybersecurity without risking my main computer.

## Proof

Add a screenshot of the Linux desktop or terminal here.
````

---

## Day 5 Deliverable

By the end of Day 5, the project should have:

- A working Linux virtual machine
- A screenshot proving the lab opened
- A short markdown note explaining what was done
- Three basic Linux commands documented
- A clear explanation of why the lab is safe for practice

This is enough.

Do not overbuild today.

Do not turn this into a three-hour setup nightmare.

The win is simple:

> The lab opens.  
> Linux runs.  
> The learner types commands.  
> The work gets documented.

---

## Suggested File Name

```text
day-05-starting-the-cybersecurity-lab.md
```

Suggested folder:

```text
days/day-05-starting-the-cybersecurity-lab.md
```

---

## Day 5 Summary In My Voice

Day 5 was about getting the cybersecurity lab moving for real. Not theory, not pretending, not just watching somebody else do it. I opened the virtual machine, got into Linux, and started using basic commands like `whoami`, `pwd`, and `ls`. The point was not to become some expert overnight. The point was to prove that I can build a safe space to practice, make mistakes, and learn cybersecurity step by step. This is where the lab starts becoming real.
