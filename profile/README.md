# Welcome to LearnToCodeSec!

Hey! I thought I'd put together a document for some basic concepts around Git and Github. I've created this guide to help us understand the essential tools we'll be using in our projects. Whether you're just starting out or have some programming experience, this guide will help you understand how we'll collaborate and learn together using Git and GitHub. This guide will help you understand the fundamental concepts of version control, the differences between Git and GitHub, and how to effectively contribute to projects. Whether you're new to development or just need a refresher, this should have something for you.

## Git vs GitHub: Understanding the Difference

Think of Git as your personal photo album manager, and GitHub as a social media platform for sharing those albums.

### What is Git?

Git is a distributed version control system that runs on your local computer. It helps you track changes in your code, similar to how Google Docs tracks changes in a document. Some key things Git does:

- Records a history of all changes made to your code
- Allows you to work on different versions of your code simultaneously
- Helps manage conflicts when multiple people edit the same file
- Works completely offline on your local machine

For example, when you save a file in a regular editor, you only have the latest version. With Git, you have a complete history:

```
// Regular saving
Document_v1.txt → Document_v2.txt → Document_v3.txt

// With Git
Initial commit → Added feature A → Fixed bug → Added feature B
     ↓              ↓               ↓            ↓
All versions are preserved and can be accessed at any time
```

### What is GitHub?

GitHub is a web platform that hosts Git repositories and adds collaboration features on top of Git. It provides:

- A central place to store your code online (remote repository)
- Tools for code review and discussion
- Project management features
- Access control and security
- Integration with other development tools

## Core Concepts in Modern Development

### 1. Repositories (Repos)

A repository is like a project folder that contains all your code and its history. For example:

```
your-awesome-project/
├── src/
│   ├── main.js
│   └── helpers.js
├── README.md
└── .git/          <- This hidden folder contains all Git history
```

### 2. Issues

Issues are like a project's to-do list. They help track:

- Bugs that need fixing
- New features to add
- Improvements to make

Example of a good issue:

```markdown
Title: Create a fun number guessing game

Description:
Let's build a simple game where the computer picks a random number 
and the player tries to guess it! This will be a great first project 
to learn about user input, loops, and conditionals.

Learning Objectives:
- Work with basic Python syntax
- Learn about while loops
- Practice using if/else statements
- Handle user input

Acceptance Criteria:
- Computer generates a random number between 1-100
- Player can input their guess
- Game provides "higher" or "lower" hints
- Congratulate player when they win
- Track number of attempts
- Add encouraging messages for players

Bonus Ideas:
- Add difficulty levels
- Keep track of high scores
- Add colorful console output
```
Related: [Higher Lower Guessing Game](https://github.com/LearnToCodeSec/beginner-projects?tab=readme-ov-file#higher-lower-guessing-game)

### 3. Branches and Pull Requests

Branches let you work on new features without affecting the main code. Think of it like creating a copy of your document before making major changes.

Creating a new branch:
```bash
# Create and switch to a new branch
git checkout -b feature/dark-mode

# Make your changes and commit them
git add new_file.py
git commit -m "Add dark mode toggle and styles"

# Push your changes to GitHub
git push origin feature/dark-mode
```

Once your changes are ready, you create a Pull Request (PR) on GitHub to propose merging your changes into the main codebase.

### 4. Code Reviews

Code reviews are a way of having people sanity check your work. They help:

- Catch bugs early
- Ensure code quality
- Share knowledge among team members
- Maintain consistent coding standards

Example of a good code review comment:
```
In src/theme.js:
Consider using CSS custom properties instead of hardcoded color values. 
This would make it easier to switch between themes:

Before:
.dark-mode { background-color: #1a1a1a; }

After:
:root {
  --bg-dark: #1a1a1a;
  --bg-light: #ffffff;
}
.theme-dark { background-color: var(--bg-dark); }
```

### 5. Approvals and Merging

Before code can be merged into the main branch, it typically needs:

1. All automated tests to pass (if you have any)
2. Required number of approvals from reviewers
3. No unresolved comments
4. Up-to-date with the main branch

Think of it like a checklist before publishing a book:
- Editor's review ✓
- Proofreading ✓
- Format check ✓
- Final approval ✓

## Best Practices

1. **Commit Messages**: Write clear, descriptive commit messages that explain why a change was made:
   ```
   Good: "Add input validation to prevent SQL injection"
   Bad: "Fix bug"
   ```

2. **Branch Names**: Use consistent branch naming:
   ```
   feature/add-dark-mode
   bugfix/fix-login-error
   docs/update-readme
   ```

3. **Pull Request Size**: Keep PRs focused and reasonably sized:
   - One PR should address one concern
   - Aim for less than 500 lines of code when possible
   - Break large changes into smaller, logical PRs

4. **Code Review Etiquette**: When reviewing code:
   - Be constructive and specific
   - Explain your reasoning
   - Suggest improvements, don't just point out problems
   - Respond to all comments before merging

## Getting Started

1. Install Git on your computer (from git-scm.com)
2. Set up your GitHub account
3. Clone this repository:
   ```bash
   git clone https://github.com/LearnToCodeSec/your-repo.git
   ```
4. Create a new branch for your work
5. Make changes and commit them
6. Push your changes and create a Pull Request

Remember, everyone was a beginner once. Don't hesitate to ask questions in issues or pull request comments.

## Getting Started Together

Since we work together, we have some advantages in learning to code:

1. **Hands-on Support**
   - We can pair program during lunch breaks
   - Quick desk-side help when you're stuck on a problem
   - A discord channel to keep up to date with what people are working on

2. **Workplace Projects**
   - Practice with real-world scenarios from our daily work
   - Build tools that could help our team (but not in work time!)
   - Learn concepts that are relevant to our industry

3. **Collaborative Learning**
   - Share knowledge in the Discord channel
   - Work on group projects together
   - Learn from each other's different perspectives and experiences

### Resources and Support

I've forked a few repositories that might help you with some initial project ideas and concepts:

- Our [python-coding-fundamentals](https://github.com/LearnToCodeSec/python-coding-fundamentals) repository contains basic concepts and exercises
- The [beginner-projects](https://github.com/LearnToCodeSec/beginner-projects) repository lists potential projects you can start working on now
- The [project-based-learning](https://github.com/LearnToCodeSec/project-based-learning) and [Projects](https://github.com/LearnToCodeSec/Projects) repos to help you with some project ideas

### Getting Help

1. Reach out on our Microsoft Teams chat or message directly
2. Ask me when I'm in the office
3. Drop a message into the discord chat
4. Add comments or questions to any repository

Remember: We're learning together, and there's no such thing as a silly question.