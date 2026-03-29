# Voice Calibration Prompt

Use this prompt to generate a personalized Part 2 for your `SKILL.md`. Paste it into any AI tool (Claude, ChatGPT, Gemini, etc.) along with 3-5 samples of your own writing (emails, essays, cover letters, blog posts, anything you wrote yourself).

---

## The Prompt

Copy everything below and paste it into your AI tool, followed by your writing samples.

```
Analyze the writing samples below and extract my personal voice profile. I need this to configure a writing style skill for my AI tool.

For each category below, give me concrete patterns you observe in MY writing. Be specific. Quote phrases I actually used. Don't describe what good writing looks like in general. Describe what MY writing looks like.

IMPORTANT: If there isn't enough data to confidently identify a pattern for a category, say "Not enough data to determine" instead of guessing. A wrong pattern is worse than no pattern. If I only provided one or two short samples, flag that upfront and recommend I add more before using the profile.

Also note my register range: do I write differently across formal vs. informal samples? If so, describe both registers and when each applies.

Output the result as directives (e.g., "Use short sentences," "Open with a scene") — NOT as descriptions of the user (e.g., "You tend to write short sentences"). The output will be pasted into an AI system prompt, so it must read as instructions the AI can follow directly.

Use this exact markdown format so I can paste it directly into my SKILL.md:

### Sentence structure
[Directives on sentence length, clause connection, and rhythm. Quote example patterns from my samples.]

### Paragraph structure
[Directives on paragraph length, transitions, and how to organize points.]

### How to open
[Directives on how to start a piece. Quote my actual openings as models.]

### How to use numbers
[Directives on how to present numbers — casually, dramatically, clustered, etc.]

### How to connect to companies/people
[Directives on how to show interest or establish relevance when writing to someone.]

### How to close
[Directives on how to end a piece. Quote my actual closings as models.]

### Words and phrases to use
[List real phrases from my samples. Note patterns like "use X instead of Y."]

### Things to never do
[Stylistic choices to avoid, based on what I consistently avoid across all samples.]

### Register range
[Directives on how to shift tone between formal and informal contexts. Note baseline register.]

---

Here are my writing samples:

[PASTE YOUR WRITING SAMPLES HERE]
```

---

## Tips for good results

- **More samples = better profile.** 3 is the minimum. 5-8 is ideal.
- **Mix formats.** Include both formal (cover letter, essay) and informal (email, message) writing so the AI captures your range.
- **Use writing you're proud of.** Don't include drafts you weren't happy with.
- **Include at least one long piece** (500+ words) so the AI can see your paragraph and transition patterns.
- **Review the output.** The AI might surface patterns you didn't notice. Keep what feels right, cut what doesn't.

## After generating

1. Open `write-like-a-human/SKILL.md`
2. Find **Part 2: Voice Profile**
3. Replace the `[USER: ...]` placeholder with the generated output
