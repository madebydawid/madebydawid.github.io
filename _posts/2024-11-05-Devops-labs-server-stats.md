---

title: Server Performance Stats Tool

date: 2024-11-05 13:40 +0200

categories: [DevOps, Monitoring]

tags: [linux, shell_scripting, monitoring, performance_analysis]

---

  

<div style="background-image: url('https://images.unsplash.com/photo-1488590528505-98d2b5aba04b?q=80&w=2670&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');

            background-size: cover;

            background-position: center;

            width: 100%;

            height: 300px;">

</div>

  
  

# Server Performance Stats Tool

  

This project focuses on creating a script that gathers and displays essential performance statistics from any Linux server. The goal is to deepen my understanding of server monitoring and improve my shell scripting skills. I love working in Linux environment and in Bash cli, but I feel that my scripting skills leave a lot of room for improvement, thus this project was lots of fun and learning.
I am nowhere near a professional scripting-king but I did solve the task nontheless, albeit with the help of LLM's 😊

  

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

  

This tool serves as a practical way to monitor server performance and is especially useful for early-stage diagnostics. For more details on this project, check out my roadmap entry on [server performance stats](https://roadmap.sh/projects/server-stats).