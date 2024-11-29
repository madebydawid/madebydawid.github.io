---
title: Linux Log Archive Tool
date: 2024-11-26 10:40 +0200
categories: [Linux, DevOps]
tags: [linux, shell_scripting, archive, logging]
---

<div style="background-image: url('https://images.unsplash.com/photo-1714846201670-1c5721196c7a?q=80&w=2574&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
            background-size: cover;
            background-position: center;
            width: 100%;
            height: 250px;">

</div>
 
# Project 02/21
So, in this project, I created a tool that archives old logs on a schedule. It compresses the logs into .tar.gz files and stores them in a separate directory for better organization and storage efficiency.

This project allowed me to strengthen my Linux and shell scripting skills, tackle automation challenges, and explore concepts that are foundational to DevOps practices.


---

## Project Goal
The goal of this project was to develop a simple yet functional log archiving tool for Linux systems. The tool automates the process of compressing and storing old logs, ensuring they are easily accessible while freeing up space in the primary log directory.


## Requirements
The tool needed to meet the following requirements:

Archive Logs: Compress all old logs in a specified directory into a .tar.gz archive.
Scheduled Archiving: Provide an option to schedule log archiving at regular intervals.
Logging the Process: Keep a record of when logs were archived, for future reference.
Easy to Use: Accept input parameters for the log directory and archive destination.

## How to Use It
Using the tool is straightforward:

Clone the repository from GitHub: [Log-Archive-Tool](https://github.com/madebydawid/Log-Archive-Tool).
Run the script with the required arguments, such as the log directory and the desired archive location.
(Optional) Set up a cron job to automate the process at regular intervals. Instructions are included in the repository's README file.

## How did I approach the challenge?
I did some online research and used LLMs to guide me by suggesting steps without providing direct answers—unless I specifically asked for them.
Although I had some prior experience with ``.tar.gz`` files from practicing ethical hacking on [TryHackMe.com](www.tryhackme.com), I still needed to look up the correct syntax.

But with some help from my AI-robot LLM friends and google-ninja stuff I finished the project with great success.

## What did I Learn?
This project was an excellent learning experience, and I gained valuable insights, including:

Linux Commands 🐧: Deepened my understanding of commands like ``tar``, ``find``, and ``crontab``.
Shell Scripting 📜: Improved my ability to write efficient and reusable scripts.
Automation 🤖: Learned the importance of scheduling workflows.
Problem-Solving 🛠️: Developed strategies to debug and troubleshoot unexpected issues during script execution.
