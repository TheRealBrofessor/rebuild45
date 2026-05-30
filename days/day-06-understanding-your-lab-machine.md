# Day 6: Understanding Your Lab Machine

## Theme

Before we use the lab for cybersecurity practice, we need to understand what kind of machine we are practicing on.

Day 6 is about taking inventory.

Not in a complicated way.

Not like an enterprise IT department.

Just enough to understand the basic parts of the Linux virtual machine and what those parts mean.

---

## Core Goal

By the end of today, the learner should understand:

- What a hostname is
- What an operating system is
- What CPU means
- What memory means
- What disk space means
- How to check basic system information in Linux
- Why knowing your lab machine matters before doing cybersecurity work

---

## Plain-English Explanation

A cybersecurity lab is still a computer.

Before we start scanning, testing, reading logs, or building tools, we should know what we are working with.

Think of it like buying a used car.

Before driving it across the country, you would want to know a few basic things:

- What kind of engine does it have?
- How much gas is in it?
- Are the tires okay?
- What does the dashboard say?

Your Linux lab machine is the same idea.

Today we are checking the dashboard.

We are not trying to memorize every detail.

We are learning how to ask the machine basic questions and read the answers.

---

## What We Are Checking Today

Today we will check:

```text
User
Hostname
Operating system information
CPU information
Memory usage
Disk space
Current location in the file system
```

These are basic details, but they matter.

Cybersecurity work depends on knowing what system you are working inside.

If you do not know what machine you are using, what user you are logged in as, or how much space you have, you are guessing.

REBUILD45 is not about guessing.

It is about learning how to verify.

---

## Important Mindset

You do not need to understand every line of output today.

Some commands will print a lot of information.

That is normal.

The goal is not to become a Linux expert in one day.

The goal is to stop seeing the terminal as a wall of mystery.

Today you are learning this:

> I can ask Linux questions, and Linux will answer.

That is a big step.

---

## Step 1: Open the Terminal

Start your Linux virtual machine.

Open the terminal.

The terminal is where we type commands and receive text-based answers from the system.

You already used a few commands on Day 5:

```bash
whoami
pwd
ls
```

Today we are going to add a few more.

---

## Step 2: Check Who You Are Logged In As

Type:

```bash
whoami
```

This shows the current user account.

You may see something like:

```bash
rebuild45
```

or:

```bash
student
```

or the username you created.

### Plain-English Meaning

This command answers:

> Who am I on this machine right now?

That matters because different users can have different permissions.

In cybersecurity and Linux, permissions matter a lot.

---

## Step 3: Check the Machine Name

Type:

```bash
hostname
```

This shows the name of your Linux machine.

You may see something like:

```bash
rebuild45-lab
```

or whatever name was assigned during setup.

### Plain-English Meaning

A hostname is the computer’s name on the system or network.

Just like people have names, computers can have names too.

When you build labs with multiple machines later, hostnames help you tell them apart.

---

## Step 4: Check the Operating System and Kernel

Type:

```bash
uname -a
```

This prints system information about Linux.

You may see a long line of text.

Do not panic.

You do not need to understand every word yet.

### Plain-English Meaning

This command answers:

> What kind of Linux system am I running?

The word `kernel` may appear or be represented in the output.

The kernel is the core part of the operating system that helps the software and hardware talk to each other.

Simple version:

> The kernel is one of the deepest, most important parts of Linux.

You do not need to master that today.

Just know that `uname -a` gives you basic system identity information.

---

## Step 5: Check CPU Information

Type:

```bash
lscpu
```

This shows information about the processor.

The processor is often called the CPU.

CPU stands for:

```text
Central Processing Unit
```

### Plain-English Meaning

The CPU is the part of the computer that does the thinking and processing.

For your virtual machine, this command shows what CPU resources the VM can see.

You may see information about:

- CPU architecture
- Number of CPU cores
- CPU model
- Virtualization support

You do not need to memorize it.

Just notice that Linux can report this information directly from the terminal.

---

## Step 6: Check Memory Usage

Type:

```bash
free -h
```

This shows memory usage in a human-readable format.

The `-h` means human-readable.

That usually means the output is easier to read, using sizes like MB or GB.

### Plain-English Meaning

Memory is the short-term working space your computer uses while programs are running.

If storage is like a filing cabinet, memory is like the top of your desk.

The more desk space you have, the more things you can work on at once.

The `free -h` command helps you see how much memory is available and how much is being used.

---

## Step 7: Check Disk Space

Type:

```bash
df -h
```

This shows disk space usage.

Again, the `-h` means human-readable.

### Plain-English Meaning

Disk space is the long-term storage area of the system.

This is where files, programs, logs, screenshots, and notes are stored.

If memory is the top of your desk, disk space is the filing cabinet.

This command helps answer:

> How much storage does this machine have left?

That matters because labs can create files, logs, screenshots, and scan results.

You do not want to blindly fill up your lab machine.

---

## Step 8: Save the Commands Used Today

Create or update your Day 6 lab notes with the commands you ran:

```bash
whoami
hostname
uname -a
lscpu
free -h
df -h
```

These commands give you a basic system inventory.

That means you now have a simple way to check what machine you are working on.

---

## First Commands Used Today

| Command | Plain-English Meaning |
|---|---|
| `whoami` | Shows the current logged-in user |
| `hostname` | Shows the computer name |
| `uname -a` | Shows Linux system information |
| `lscpu` | Shows CPU information |
| `free -h` | Shows memory usage in an easier format |
| `df -h` | Shows disk space usage in an easier format |

---

## Beginner Safety Note

Today’s commands are safe because they only read information.

They do not delete files.

They do not change system settings.

They do not install tools.

They simply ask Linux questions and show the answers.

That is a good habit to build early:

> Read first. Understand first. Change later.

---

## What To Document Today

Create a short Day 6 note with:

````markdown
# Day 6 Lab Notes

## What I Did

Today I checked basic information about my Linux lab machine.

## What I Learned

I learned that Linux can show information about the user, hostname, operating system, CPU, memory, and disk space from the terminal.

## Commands I Used

```bash
whoami
hostname
uname -a
lscpu
free -h
df -h
```

## What I Understand Now

I understand that before doing cybersecurity work, I should know what machine I am working on and what resources it has.

## Proof

Add a screenshot of the terminal output here.
````

---

## Day 6 Deliverable

By the end of Day 6, the project should have:

- A basic inventory of the Linux lab machine
- A screenshot of terminal output
- A markdown note explaining what was checked
- A beginner-friendly explanation of CPU, memory, disk space, hostname, and operating system information
- A better understanding of why verification matters

This is enough.

Do not overcomplicate this.

The win is simple:

> I opened the lab.  
> I checked the machine.  
> I understood more than I did yesterday.  
> I documented the proof.

---

## Suggested File Name

```text
day-06-understanding-your-lab-machine.md
```

Suggested folder:

```text
days/day-06-understanding-your-lab-machine.md
```

---

## Day 6 Summary In My Voice

Day 6 was about learning what kind of machine I am actually working on. Instead of just opening Linux and guessing, I used commands like `whoami`, `hostname`, `uname -a`, `lscpu`, `free -h`, and `df -h` to check the lab machine. I learned how to see the user, computer name, system information, CPU, memory, and disk space. This was not flashy, but it matters. Cybersecurity starts with knowing what system you are touching before you start changing things.
