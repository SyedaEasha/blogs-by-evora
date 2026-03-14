---
title: "Git and GitHub"
date: 2026-03-13
draft: false
author: "Syeda Easha"
description: "A beginner friendly guide to Git, GitHub and pushing your first repository."
tags: ["Git", "GitHub", "Version Control", "Ubuntu"]
categories: ["Tech Blogs"]
---

## Introduction

Git and GitHub are two essential tools for developers. They help track changes in projects, collaborate with others, and manage code efficiently.

In this blog, we will understand the concept of version control systems, install Git on Ubuntu, generate an SSH key, and push a project to GitHub.

---

## Concept of Version Control System

A **Version Control System (VCS)** helps developers manage and track changes in source code over time.

It allows you to:

- track file changes
- revert to previous versions
- collaborate with others
- maintain a history of project development

There are two main types of version control systems.

### Centralized Version Control

In centralized systems, all developers connect to a central server where the project history is stored.

### Distributed Version Control

In distributed systems, every developer has a complete copy of the repository history on their local machine.

Git is a **distributed version control system**.

---

## Introduction to Git

Git is a popular version control tool used by developers to manage and track code changes.

Git allows developers to:

- track project history
- collaborate with teams
- experiment safely using branches
- revert mistakes easily

---

## Git Terminology

### Repository

A repository is a storage location where your project files and version history are saved.

### Staging Area

The staging area holds changes that will be included in the next commit.

### Commit

A commit is a snapshot of your project at a specific time.

### Branch

Branches allow developers to work on different features without affecting the main code.

### Remote

A remote repository is a version of your project hosted online.

Example: GitHub.

### Clone

Cloning means downloading a complete copy of a repository to your local machine.

---

# Installing Git on Ubuntu

## Step 1: Update Packages

First update your package list.
sudo apt update


## Step 2: Install Git


sudo apt install git -y


## Step 3: Verify Installation


git --version


If a version number appears, Git has been installed successfully.

---

## Step 4: Configure Git

Set your username:
git config --global user.name "Your Name"


Set your email:


git config --global user.email "youremail@example.com
"
## Step 5: Check Git Configuration


git config --list


---

# GitHub on Ubuntu

## What is GitHub?

GitHub is a cloud platform used to host Git repositories online. It helps developers store projects, collaborate with teams, and manage version history.

---

## Create a GitHub Account

1. Go to **github.com**
2. Click **Sign Up**
3. Enter your email, username, and password
4. Verify your email

---

# Generate an SSH Key

SSH keys allow your computer to communicate securely with GitHub.

Generate an SSH key:


ssh-keygen -t ed25519 -C "youremail@example.com
"


Press **Enter** to save the key in the default location.

Start the SSH agent:


eval "$(ssh-agent -s)"


Add the SSH key:


ssh-add ~/.ssh/id_ed25519


Copy your public key:


cat ~/.ssh/id_ed25519.pub


Add the copied key to **GitHub → Settings → SSH Keys**.

---

# Create and Push a Repository

## Step 1: Create a Project Folder


mkdir learning
cd learning


---

## Step 2: Create a File


echo "Hello GitHub" > readme.txt


---

## Step 3: Initialize Git Repository


git init


---

## Step 4: Add Files


git add .


---

## Step 5: Commit Changes


git commit -m "Initial commit"


---

## Step 6: Add Remote Repository


git remote add origin git@github.com
:yourusername/learning.git


---

## Step 7: Verify Remote


git remote -v


---

## Step 8: Push to GitHub


git push -u origin main


Now open your GitHub repository and you should see your project files uploaded successfully.

---

# Final Thoughts

Git and GitHub are essential tools for every developer. Learning how to manage repositories, commit changes, and push code to GitHub will greatly improve your development workflow.

Whether you are working alone or in a team, Git makes project management easier and more organized.

---


