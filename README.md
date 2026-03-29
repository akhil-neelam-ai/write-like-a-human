# Write Like a Human

You just asked an AI to write an email. It came back with this:

> *We are delighted to present this comprehensive overview, which delves into the intricacies of our innovative approach. The initiative not only enhanced operational efficiency — it fundamentally transformed how the organization fosters collaboration, innovation, and growth.*

Nobody talks like that. Your reader knows it. Your recruiter knows it. Your professor knows it.

This skill fixes it.

## What it is

A single markdown file you drop into any AI tool. It rewrites how the AI writes — killing the patterns that scream "a machine made this" and replacing them with prose that sounds like you sat down and typed it yourself.

Works with **Claude, ChatGPT, Gemini, Manus**, and anything else that takes a system prompt.

## What it catches

| AI Tell | Before | After |
|---|---|---|
| Banned words | "delve into the intricacies" | "dig into the details" |
| Em dash overuse | "not just scale -- but impact" | "The scale matters. But what kept me going was seeing it work." |
| Rule of three | "innovation, collaboration, and impact" | "I wanted to build something that worked." |
| Dangling -ing | "...fostering a sense of community" | Delete it. |
| Puffery | "an astonishing 85% reduction" | "cutting load by 85%" |
| Formulaic opener | "Additionally, the team..." | "The team..." |
| Chatbot leakage | "I hope this helps!" | Remove from drafted content. |
| Uniform rhythm | Three 12-word sentences in a row | Mix a 4-word fragment with a 25-word sentence |
| Positivity bias | "challenges ultimately strengthened the team" | "We broke prod twice. The new system is faster." |
| No engagement | All third-person declarative statements | Add a question, "we," or direct address |

50+ banned words. 13-point self-check with before/after examples. A substitution table for quick swaps.

Built on research from [Mapping the Increasing Use of LLMs in Scientific Papers](https://arxiv.org/abs/2404.01268) (950,000+ papers analyzed), [EMNLP 2024 syntactic template study](https://aclanthology.org/2024.emnlp-main.368/), [GPTZero's burstiness/perplexity framework](https://gptzero.me/news/how-ai-detectors-work/), and other research.

## Make it sound like *you*

Out of the box, the skill defaults to short sentences, simple verbs, and concrete details. Good enough for most people. But if you want the AI to match your specific voice, there's a calibration step.

1. Open [`CALIBRATE.md`](CALIBRATE.md)
2. Copy the prompt. Paste it into any AI tool with 3-5 samples of writing you've already done.
3. The AI analyzes your patterns and generates a voice profile: your sentence structure, your openers, your word choices, your register range.
4. Paste the output into Part 2 of `SKILL.md`.

Now every piece of writing the AI produces starts from your voice, not a generic "professional" one.

## How to use

One file: `write-like-a-human/SKILL.md`. Drop it into your tool.

### Claude (Desktop / Web)

1. Go to Settings > Skills
2. Click "+" and upload `write-like-a-human/SKILL.md`

Activates automatically on any prose task.

### Claude Code

```bash
mkdir -p ~/.claude/skills/write-like-a-human
cp write-like-a-human/SKILL.md ~/.claude/skills/write-like-a-human/SKILL.md
```

Then add to your project's `CLAUDE.md`:

```markdown
**Always apply the writing style skill (`~/.claude/skills/write-like-a-human/SKILL.md`) when generating any prose.**
```

### ChatGPT

**Custom Instructions** (all chats): Profile > Settings > Personalization > Custom Instructions. Paste into "How would you like ChatGPT to respond?" (1,500 char limit — trim to key rules).

**Custom GPT** (dedicated, 8,000 chars): Profile > My GPTs > Create a GPT. Paste full contents into Instructions.

### Gemini

**Saved Instructions** (all chats, needs Advanced): Settings & help > Personal Intelligence > Instructions for Gemini. Paste contents.

**Gem** (dedicated, needs Advanced): Gem Manager > New Gem. Paste into Instructions, or upload as a knowledge file.

### Manus

Create a Project > set Master Instruction. Paste contents. Optionally upload to Knowledge Base.

### Any other LLM

Paste into the system prompt or custom instructions. It's plain markdown. Works anywhere.

## License

MIT
