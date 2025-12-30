# Ponder

This is a Claude Code plugin that helps enhance your prompts. It analyses your repo's files, asks you some questions and sends Claude an enhanced version of your prompt.

## How to install

First add the marketplace:
```bash
claude plugin marketplace add integralbyte/ponder-cc
```

Then install the plugin:
```bash
claude plugin install ponder@ponder-cc
```

## Commands

- `/ponder:enhance`: The main command. You give it a task, it analyses the repo, asks you some follow-up questions, and then lets you review the plan before it runs.

## Usage

Run the `/ponder:enhance` command followed by your prompt:

```bash
/ponder:enhance add authentication to my app
```

## How it works

1. It looks at your config files and project structure.
2. If your request is vague, it asks you which tools or files you want to use. It also asks you the desired level of detail for the enhanced prompt.
3. It generates and shows you the prompt before proceeding.
4. If you select yes, it sends Claude the enhanced version prompt.
