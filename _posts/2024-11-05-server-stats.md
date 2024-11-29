---
title: Server Performance Stats Tool
date: 2024-11-05 10:40 +0200
categories: [Linux, DevOps, Monitoring]
tags: [linux, shell_scripting, monitoring, performance_analysis]
---

<div style="background-image: url('https://images.unsplash.com/photo-1629654297299-c8506221ca97?q=80&w=2574&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
            background-size: cover;
            background-position: center;
            width: 100%;
            height: 250px;">

</div>
 
# Project 01/21
This project focuses on creating a script that gathers and displays essential performance statistics from any Linux server. The goal is to deepen my understanding of server monitoring and improve my shell scripting skills. I love working in Linux environment and in Bash cli, but I feel that my scripting skills leave a lot of room for improvement, thus this project was lots of fun and learning.
I am nowhere near a professional scripting-king but I did solve the task nonetheless, albeit with the help of LLM's 😊

---

## Project Goal

The primary objective of this project is to write a script, `server-stats.sh`, to analyze and display basic server performance stats in a clear format. This script allows for quick insights into server health and helps identify potential issues by focusing on resource usage and top processes.

## Requirements

The `server-stats.sh` script should be capable of providing the following server statistics:

- **Total CPU usage**
- **Total memory usage** (Free vs. Used, including percentage)
- **Total disk usage** (Free vs. Used, including percentage)
- **Top 5 processes by CPU usage**
- **Top 5 processes by memory usage**

**Stretch Goal**: Additional information like OS version, uptime, load average, logged-in users, and failed login attempts can be added for further insight into the server status.

## How to Use It
To run the `server-stats.sh` script on any Linux server, follow these steps:

1. Log in to your Linux server.
2. Copy the code from `server-stats.sh`.
3. Run `sudo nano server-stats.sh` to create the script file.
4. Paste the copied code into the file.
5. Save the file by pressing `Ctrl + X`, then `Y`, and `Enter`.
6. Change the file permissions to make it executable: `chmod +x server-stats.sh`.
7. Run the script with the following command: `./server-stats.sh`.

---

## How did I approach the challenge?
While I have some familiarity with Linux and the Bash shell, I’m still finding my way around scripting, especially in the CLI. When it comes to writing scripts, I must admit this was my first serious attempt. To make the most of it, I decided to use an LLM (Large Language Model) as a guide to help me structure this project as both a practical task and a learning experience.

I enlisted ChatGPT as my tutor, asking it to “hold my hand” without giving away all the answers, guiding me step-by-step through the project so I could absorb the essentials. The project itself provided a good roadmap, especially in terms of which commands I’d need, so I had a solid starting point.

It took me a few hours to complete the script, and I now feel more comfortable reading Bash code. I know there’s still a long way to go before I can confidently script independently, but hey, it’s a start! 👍



## What did I Learn?

First off, I learned a practical tip: *define variables before you use them!* 😄 This exercise also gave me a great insight into Bash’s flexibility. It’s quite powerful and capable of some cool tricks, like changing text color to enhance readability.

Now, with this script in hand, I can use it for future projects or even in production environments if needed—which in itself is pretty exciting. ⚡
