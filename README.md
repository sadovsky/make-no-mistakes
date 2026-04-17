# make-no-mistakes

The most important Claude Code plugin ever designed by human hands.

## The Problem

Claude is pretty good. But is it *perfect*? No. Has it ever told you that a function "should work" and then it absolutely did not work? Yes. Has it confidently hallucinated an API that has never existed? Also yes.

The root cause of all these failures has now been identified: **Claude was never explicitly told not to make mistakes.**

## The Solution

This plugin appends "Make no mistakes." to every prompt you submit.

That's it. That's the whole plugin.

Researchers estimate this single sentence increases output quality by somewhere between 0% and 100%. The error bars are wide but the commitment is real.

## How It Works

The plugin uses the `UserPromptSubmit` hook — a powerful primitive that Claude Code exposes for exactly this kind of mission-critical work — to inject "Make no mistakes." as additional context before Claude processes each prompt.

No mistakes have been made in the development of this plugin.

## Installation

```bash
# Personal use (all projects)
claude plugin install /path/to/make-no-mistakes --scope user

# Project-scoped (share the gift with your entire team)
claude plugin install /path/to/make-no-mistakes --scope project
```

## Testing Without Installing

```bash
claude --plugin-dir /path/to/make-no-mistakes
```

Submit any prompt. Observe Claude making no mistakes. You're welcome.

## FAQ

**Q: What if Claude makes a mistake anyway?**
A: That's on you for not installing this plugin sooner.

**Q: Should this be in my company's standard developer setup?**
A: Absolutely. Add it to your onboarding docs immediately.

**Q: Is this peer-reviewed?**
A: It has not been *not* peer-reviewed.

## License

MIT
