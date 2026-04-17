# make-no-mistakes

A Claude Code plugin that appends "Make no mistakes." to every prompt you submit.

## How It Works

The plugin uses the `UserPromptSubmit` hook to inject "Make no mistakes." as additional context before Claude processes each prompt.

## Installation

```bash
# Personal use (all projects)
claude plugin install /path/to/make-no-mistakes --scope user

# Project-scoped (shared via git)
claude plugin install /path/to/make-no-mistakes --scope project
```

## Testing Without Installing

```bash
claude --plugin-dir /path/to/make-no-mistakes
```

## License

MIT
