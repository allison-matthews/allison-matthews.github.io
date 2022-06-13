---
layout: post
title: Me, my shell, and I
subtitle: Tips and tricks for working in a UNIX environment
gh-repo: allison-matthews/allison-matthews.github.io
comments: true
---

If you have any questions---or discover cool UNIX tricks---please get in touch! You can email me at amatthews@carnegiescience.edu or find me in my office (#132). Mike and Peter are available at mgrudic@carnegiescience.edu and psenchyna@carnegiescience.edu and are in offices #1 and #1, respectively.

## UNIX Introduction

UNIX is an operating system first developed in the 1960s, but remains under constant development to this day. It is made up of three parts: 1. the kernel, 2. the shell, and 3. the programs. This is all about the shell---which interfaces between the kernel (the hub of the operating system) and the user (you!).
![unix](https://res.cloudinary.com/practicaldev/image/fetch/s--rpWCPbkI--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/14ajqxtcah1yx2e9kgzk.jpg)

### Why learn UNIX?
It's powerful, but don't take my word for it. The research publication _Nature_ listed ["Five reasons why researchers should learn to love the command line](https://www.nature.com/articles/d41586-021-00263-0)," summarized here:
1. **Wrangle files.** You can repeat simple tasks (like renaming, adding a date stamps, converting to a different format) across multiple files.
2. **Handle big data.** At a certain point, data sets become too big for GUI programs to handle. Using the command-line you can quickly sort through large numbers of files (>millions) and/or extract information from large files.
3. **Manipulate spreadsheets.** From the command line you can cut and extract columns, count words/lines/characters, filter files for a certain condition. Using the 'pipe' function you can combine these functions.
4. **Parallelize your work.** You almost always (maybe actually always?) interact with high performance computing systems (HPCs) through the command-line and bash scripts.
5. **Automate.** Anything you can type on the command line can be included in a bash/shell script. This means you can line up various commands to run after one-another, and you can even schedule them to run at a particular time!
### Opening a terminal: 
There are many ways to open a terminal (also called the "command line") on either Mac or Linux machines, but here are some quick options:
On a Mac: ⌘ _Cmd_ + _Space_ and type _terminal_, hit enter.
On a Linux: Click _Applications_ &rarr; _System Tools_ &rarr; _Terminal_.
On a Windows: (to-do)

There are different types of shells (e.g. `bash`, `csh`, `zcsh`, etc.), but we will be using the `bash` shell. To check what shell you're using, type: `echo $SHELL` in the terminal. `echo` teWe'lls the terminal to write the given text to screen. For example:
```bash
$ echo 'Am I a cat?'
Am I a cat?
```
The  before echo just indicates the beginning of the line on a Linux-based machine. It may differ depending on whether you are using a Linux  or a Mac machine.
