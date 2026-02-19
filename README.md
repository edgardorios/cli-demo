# This is a test

# This is the second test

---

# Setting Up Claude Code on Linux (Linux Mint)

A step-by-step guide to get Claude Code up and running on Linux Mint.

## Prerequisites

- Linux Mint (any recent version)
- Terminal access
- An Anthropic account with API access or a Claude.ai Pro/Max subscription

## Step 1: Install Node.js

Claude Code requires Node.js version 18 or higher. The recommended way is via `nvm` (Node Version Manager):

```bash
# Install nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

# Reload your shell
source ~/.bashrc

# Install the latest LTS version of Node.js
nvm install --lts

# Verify the installation
node --version
npm --version
```

## Step 2: Install Claude Code

Install Claude Code globally using npm:

```bash
npm install -g @anthropic-ai/claude-code
```

Verify the installation:

```bash
claude --version
```

## Step 3: Authenticate

Run Claude Code for the first time. It will prompt you to log in:

```bash
claude
```

This opens a browser window to authenticate with your Anthropic or Claude.ai account. Follow the on-screen instructions to complete the login.

## Step 4: Navigate to Your Project

Go to the directory you want to work on:

```bash
cd ~/your-project-folder
```

Then launch Claude Code:

```bash
claude
```

## Step 5: Start Using Claude Code

Once inside the Claude Code interactive session, you can:

- Ask Claude to explain, modify, or debug your code
- Run slash commands like `/help` to see available options
- Type your request in plain English and Claude will assist you

## Tips

- Use `claude --help` to see all available CLI flags
- You can run `claude` from any git repository and it will automatically have context of your project
- Check the [official documentation](https://docs.anthropic.com/claude-code) for advanced configuration and features
