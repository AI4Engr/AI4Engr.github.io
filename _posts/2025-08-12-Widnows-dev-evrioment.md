---
layout: post            
title: "Windows Development Environment"
date: 2025-08-17 10:00 -0500
categories: [notes]     # optional: hierarchical taxonomy
tags: [development]  # optional: free-form labels
# excerpt: "A quick start to posting with Jekyll."  # optional
published: true         # set false to hide
---

# Windows Development Environment

## Why Use Windows for Software Development
For many years, I primarily used Linux for software development at work. However, when I joined a new company, my work laptop came with Windows. At home, I also use a Windows machine for side projects and gaming. Naturally, I started looking for a solution that balanced both **software development and gaming** without constantly switching machines.

## MinGW vs WSL1/2
I rely heavily on the command line. While [WSL](https://learn.microsoft.com/en-us/windows/wsl/about) is a great option, it runs on top of **Hyper-V**, which introduces noticeable I/O performance overhead. Instead, I chose **MinGW**, which is more lightweight.  

With [MSYS2](https://www.msys2.org/), I also get the convenience of the `pacman` package manager, making updates and package installations seamless. My main development environment is **MSYS2 with MinGW64**.

Some useful commands I use frequently:

```bash
# Update everything
pacman -Syu

# Remove unused packages from cache
pacman -Sc

# Clean orphaned packages
pacman -Rns $(pacman -Qdtq)
````

## Git

One limitation of MSYS2 is Git support, especially for GUI tools like **gitk**. Meanwhile, [Git for Windows](https://git-scm.com/download/win) does not support `pacman`.

There was once a [Git for Windows SDK](https://github.com/git-for-windows/git-sdk-64), which had everything in one package, but it has been abandoned. For now, the best solution is to install **both MSYS2 and Git for Windows**, while using MSYS2/MinGW64 as the main shell.

To make Git available inside MSYS2, add this snippet to your `~/.bashrc` (replace `<install path>` with your Git installation directory):

```bash
export PATH="<install path>/Git/cmd:
<install path>/Git/mingw64/libexec/git-core:\
$PATH"
```

## Node.js

Although MSYS2/MinGW64 provides [Node.js](https://nodejs.org/), its version cannot build [Tauri](https://tauri.app/) apps for Windows. The workaround is to install the official **Windows Node.js release** and then update your `~/.bashrc`:

```bash
export PATH="/c/Program Files/nodejs:$PATH"
```

This ensures Node works properly for Tauri and other native builds.

## Meld

I use [Meld](https://meldmerge.org/) for file and folder comparison. Installing it inside MSYS2/MinGW64 means I can keep it updated easily with `pacman`.

To use **Meld** directly in a Windows terminal or PowerShell, add the MSYS2 `bin` directory to your system PATH:

```bash
set PATH=C:\msys64\mingw64\bin;%PATH%
```

## Python

I recommend to use [conda-forge](https://conda-forge.org/) or [miniforge](https://conda-forge.org/_download/)

## CMake/Emacs

I installed them inside MSYS2/MinGW64 and use them everywhere

## Final Thoughts

With this setup:

* **MSYS2/MinGW64** gives me a Linux-like environment.
* **Git for Windows** fills the Git GUI gap.
* **Windows Node.js** ensures compatibility for Tauri and native builds.
* **Meld** integrates seamlessly for diff/merge tasks.

This way, I get the best of both worlds: a smooth development experience on Windows while keeping gaming performance intact.










