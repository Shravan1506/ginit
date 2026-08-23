# GINIT - Your First Introduction to GitHub!

This repository is an initial introduction to GitHub! Let's get started with some basics!

## What is Github?

GitHub is a tool for code storage and management. You can use GitHub by creating an account. It's free but unfortunately not Open Source, it's built on top of Git, the FOSS tool. To put it simply, GitHub lets you store your projects online, track changes to your code, and collaborate with others. It also provides features like repositories, branches, issues, and pull requests to make managing projects easier.

## Getting started!

To download Git, use the following links:

- [Git for Windows](https://git-scm.com/install/windows)
- **Unix/Linux:** Git is usually available through your system's package manager.

Then configure Git with your name and email:

```sh
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### SSH setup (Optional but Highly Recommended!)

For setting up SSH, please follow the steps given in [SSH setup](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).

## Cloning a Repository

First, clone this repository locally using one of the following methods:

### HTTPS Method

This requires no SSH setup but may require additional authentication:

```sh
git clone https://github.com/Team-Proboticists/ginit.git
```

### SSH Method

Requires setup of an [SSH key](#ssh-setup).

```sh
git clone git@github.com:Team-Proboticists/ginit.git
```

**SSH is the preferred method.**

## Directory Description

As you can see, this directory contains a `README.md` along with some folders:

```text
.
├── cppCodes
│   └── main.cpp
├── pythonCodes
│   └── main.py
└── README.md
```

# Your First Git Workflow

Now let's actually use Git!

## Branches

A **branch** is essentially your own version of the project where you can make changes without affecting the main project.

First, create a new branch using:

```sh
git checkout -b your-name
```

You can check which branch you are currently on using:

```sh
git branch
```

## Make Your Changes

Your task is to create a file called:

```text
README.md
```

Inside it, write a short introduction about yourself. You can include things like:

- Your name
- Your department/year
- Your interests
- Your hobbies
- Your favourite programming language
- Anything else you think is interesting!

Along with it, add your photo, so that we can use it for our socials!

## Check Your Changes with `git diff`

Before committing your changes, you can see exactly what has changed using:

```sh
git diff
```

`git diff` shows the differences between your current files and the last committed version.

This is useful for checking what you're about to commit.

## Commit Your Changes

Once you're happy with your changes, tell Git to start tracking the file:

```sh
git add README.md
```

Then create a **commit**:

```sh
git commit -m "Add my about me"
```

A commit is essentially a snapshot of your project at a particular point in time.

## Push Your Branch

Your branch currently only exists on your computer. To upload it to GitHub:

```sh
git push -u origin your-name
```

Now your branch and your `README.md` file should be visible on GitHub!

## Pulling Changes

`git pull` is used to download changes from GitHub and apply them to your local repository.

```sh
git pull
```

This becomes especially important when working with other people, since they may have pushed changes while you were working.

# Your Task

1. Clone this repository.
2. Create a new branch using your name.
3. Create an `README.md` file.
4. Write a short introduction about yourself.
5. Add a nice photograph of yourself.
6. Use `git diff` to inspect your changes.
7. Commit your changes.
8. Push your branch to GitHub.
9. Open your branch on GitHub and verify that your changes are there.

### Bonus

Try creating a **Pull Request** from your branch to the `main` branch.

Don't worry if you break something. That's part of the point of using Git. Git is basically a time machine for your code.
