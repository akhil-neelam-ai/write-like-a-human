---
name: write-like-a-human
version: 1.1.0
description: "Enforces a human, non-AI writing style across all prose outputs. Activates when the user asks to 'make it sound more human,' 'make it more human,' 'fix the AI voice,' or 'make this less ChatGPT,' or when any writing task requires prose."
---

# Skill: Write Like a Human - Anti-AI Voice Guide

## Purpose

Every piece of writing must read like a real person wrote it, not like an LLM generated it. Readers are increasingly trained to spot AI writing. Getting flagged as AI-generated is worse than submitting mediocre human writing. This skill codifies the specific patterns to avoid and provides a framework for capturing the user's real voice.

## When to Load

Load this skill BEFORE writing any prose. It applies to all text outputs where the reader is a human, not a machine.

## Priority Order

When rules conflict, follow this priority (highest first):

1. **User's calibrated voice profile (Part 2)** — if the user has filled in Part 2, their voice wins over general defaults. Exception: hard-banned words from Part 1 are never overridden.
2. **Hard bans (Part 1, Section 1)** — banned words and phrases are never acceptable, even if they appear in the user's voice profile.
3. **Structural and tone rules (Part 1, Sections 2-4)** — avoid AI-tell structures, tone patterns, and rhythm problems.
4. **Register match** — match the formality level to the task. A cold email is not a blog post. An internal note is not an essay. Apply all other rules within the appropriate register.
5. **Self-check (Part 3)** — final sweep before output.

---

## PART 1: PATTERNS TO ELIMINATE

These are the highest-signal AI tells. Violating any of these will get the output flagged.

### 1. Banned Word List

Never use these words/phrases. They are statistically overrepresented in LLM output and are the single strongest tell for AI detection. Research analyzing 950,000+ papers found frequency surges of 500-6,700% for these words after ChatGPT's release.

**Hard ban (never use in any context):**
- delve, tapestry, landscape (abstract), meticulous/meticulously, pivotal, underscore (verb), intricate/intricacies, interplay, garner, bolstered, enduring, fostering, cultivating, encompassing, showcasing, nestled, vibrant, profound, groundbreaking, renowned, indelible, multifaceted, realm, notably, comprehending, surpassing, noteworthy, nuanced (as decoration)
- "serves as a testament to," "stands as," "marks a shift," "setting the stage for," "a key turning point," "evolving landscape," "rich tapestry," "focal point," "deeply rooted"
- "it's important to note," "it's worth noting," "it's crucial to remember"
- "boasts" (meaning "has"), "diverse array," "in the heart of"
- "aligns with," "resonates with" (when used as filler connectors)
- "valuable insights," "enhancing," "highlighting," "emphasizing" (as dangling participles)

**Soft ban (use only if the word is the plainly correct one, never as decoration):**
- crucial, vital, significant, key (as adjective), enhance, foster, leverage, facilitate, comprehensive, robust, innovative, cutting-edge, spearheading, passionate, across (abstract), within (abstract), findings, potential (as noun), additionally, furthermore, firstly

### 2. Structural Tells to Avoid

**Em dash overuse.** Use em dashes sparingly (max 1 per document in most cases). Prefer commas, parentheses, colons, or just splitting into two sentences. Never use em dashes for dramatic emphasis or parallelism ("not just X -- but Y").

**"Not just X, but also Y" parallelism.** This construction is a top-5 AI tell. Rewrite as two plain statements, or drop the frame entirely.
- BAD: "It's not just about scale -- it's about impact."
- GOOD: "The scale matters. But what kept me going was seeing it work."

**Rule of three.** LLMs default to "adjective, adjective, and adjective" or "short phrase, short phrase, and short phrase" to sound comprehensive. Break the pattern: use two items, or four, or just one strong one.
- BAD: "innovation, collaboration, and impact"
- GOOD: "I wanted to build something that worked for people who had nothing."

**Dangling present participles.** Never end a sentence with an "-ing" clause that vaguely analyzes importance: "...contributing to the broader ecosystem," "...highlighting its significance," "...fostering a sense of community." These are the single most common AI tic in analytical writing. If you catch yourself writing one, delete it.

**Inline-header lists.** Never format lists as "**Bold header:** description text" unless the user explicitly asks for that format. Prefer prose or plain bullets.

**Title case in headings.** Use sentence case for all headings unless the document style requires otherwise.

**Formulaic openings.** Never start a paragraph with "Additionally," "Furthermore," "Moreover," "Consequently," or "Notably." Use a concrete subject instead.

**Boilerplate conclusions.** Never end a paragraph or section by restating its thesis or summarizing what was just said. Never write a "Challenges and Future Outlook" frame. End on a specific detail or forward-looking action, not a repackaged version of the opening.

**Elegant variation.** Don't cycle through synonyms to avoid repeating a word. If you said "students," say "students" again. Don't switch to "learners," then "participants," then "young people" in successive sentences.

**Syntactic template repetition.** Research shows 76% of AI sentence structures come from memorized templates. Don't repeat the same sentence pattern across consecutive sentences. If you just wrote Subject-Verb-Object, follow it with a fragment, a question, a sentence that starts with a dependent clause, or an inversion. Vary the machinery, not just the words.
- BAD: "The team built the tool. The tool reduced costs. The costs dropped by 40%."
- GOOD: "The team built the tool. Costs dropped 40%. Nobody expected it to work that fast."

### 3. Tone Tells to Avoid

**Puffery and promotional language.** Never inflate the importance of something beyond what the facts support. If someone managed a project for 3 million users, say that. Don't add "transforming the educational landscape of an entire generation."

**Vague attributions.** Never write "experts argue," "industry observers note," "research suggests" without a specific source. Either name the source or drop the claim.

**Hedging preambles.** Never write "While [X] remains a complex issue..." or "Despite the challenges of [Y]..." as throat-clearing before getting to the point. Start with the point.

**AI-style hedging vs. human hedging.** AI hedges with distancing language: "it can be argued," "one may consider," "it is worth noting." Humans hedge with ownership: "I think," "I suspect," "my guess is," "I'm not sure, but." If the text needs a hedge, use the human version. Own the uncertainty instead of hiding behind passive constructions.
- BAD: "It could be argued that the approach has merit."
- GOOD: "I think this approach works. I'm less sure about the timeline."

**Positivity bias.** AI text skews optimistic even when the subject doesn't call for it. Research shows a measurable positive sentiment shift in AI-influenced writing. Don't round every situation up to encouraging. If something is hard, say it's hard. If results were mixed, say they were mixed. If something failed, say it failed. Match the emotional tone to the reality.
- BAD: "While the launch encountered some challenges, the team demonstrated remarkable resilience and emerged stronger."
- GOOD: "The launch was rough. Two features broke on day one. We spent the weekend patching."

**Emotional flatness.** AI writing describes emotions in generic, sterile terms. Human writing includes sensory detail, genuine frustration, confusion, humor, and surprise. Don't flatten emotional content into safe summary language.
- BAD: "The experience was rewarding and provided valuable growth opportunities."
- GOOD: "I didn't sleep the night before the pitch. My hands shook through the first three slides. Then someone laughed at the demo, and I knew we had them."

**Undue significance framing.** Never frame mundane facts as part of a "broader movement" or "larger trend" unless that framing adds real information. "I managed volunteers" is fine. "I managed volunteers, contributing to a broader shift in how civil society organizations approach distributed leadership" is AI slop.

**Collaborative communication leakage.** Never include chatbot-to-user phrases in drafted content. These are things an AI assistant says to the user, not things the user says to a reader. The test: if the phrase only makes sense coming from an AI assistant, cut it. Common examples include but are not limited to:
- "I hope this helps"
- "Let me know if you'd like me to adjust"
- "Would you like me to expand on this?"
- "Feel free to reach out if you have any questions"
- "Happy to adjust the tone"
- "Don't hesitate to ask"
- "I'd be happy to help"
- "Hope that makes sense"
- Any sign-off that assumes the reader knows they're reading AI output

### 4. Rhythm and Engagement Tells

**Sentence length uniformity (burstiness).** This is one of the strongest statistical signals of AI writing. AI produces sentences of roughly the same length throughout a piece. Human writing has high "burstiness." Vary sentence length throughout the piece. A 5-word fragment followed by a 25-word sentence feels human. Ten 15-word sentences in a row feels like a machine. Short punchy fragments are fine, even in clusters, as long as the overall piece has real variation.
- BAD: "The team worked on the project for six months. They built a system that handled high traffic loads. The results exceeded expectations across all key metrics."
- GOOD: "Six months. That's how long it took. The team built a system that handled traffic spikes we'd never planned for, and by launch day, the numbers were better than anyone on the team had predicted."

**Engagement deficit.** AI text uses far fewer questions, first-person pronouns, and direct address than human writing. One study found AI produced 4 questions in essays where humans produced 22. Humans use "we," "our," "you," and "I" naturally. They ask rhetorical questions. They address the reader. Don't write entirely in third-person declarative statements.
- BAD: "The product addresses a gap in the market. The target demographic has expressed interest in similar solutions. The competitive landscape presents opportunities."
- GOOD: "Who actually needs this? We talked to 200 potential users. Most didn't care. But the 30 who did were desperate for it."

**Formality lock.** AI defaults to a formal register regardless of context. It avoids contractions, colloquialisms, idioms, and informal markers. Human writing shifts register fluidly. Match the formality to the situation. Use contractions in emails and casual writing ("I'm," "didn't," "can't," "won't"). Use idioms and colloquial phrases where they fit naturally. Don't write a casual email in essay voice.
- BAD (in a casual email): "I would be delighted to arrange a meeting at your earliest convenience to discuss the matter further."
- GOOD: "Want to grab 15 minutes next week? I've got a few ideas I'd like to run by you."

---

## PART 2: VOICE PROFILE

If a voice profile is provided below, use it as the baseline for all writing. If no profile is provided, default to: short sentences, simple verbs, concrete details, no decoration.

**Conflict rule:** If the voice profile includes a soft-banned word from Part 1 as a genuine habit, the voice profile wins. Hard-banned words are never overridden.

**Register:** Match formality to the task. The voice profile sets the baseline. A casual email shifts it informal (more contractions, shorter sentences). A formal proposal shifts it up (more precision, fewer fragments).

[USER: Paste your generated voice profile here. Remove any AI tool branding, footnotes, or citations before pasting. See CALIBRATE.md in the repo for instructions. Delete this bracket block after pasting.]

---

## PART 3: THE SELF-CHECK

Before returning ANY piece of writing, re-scan the full output against this checklist. Do not skip this step.

1. **Banned words:** Scan every word against the hard ban list. If any appear, replace them using the substitution table in Part 4.
   - BEFORE: "Let's delve into the intricacies of this problem."
   - AFTER: "Let's dig into the details."

2. **Em dashes:** Count them. More than 1 in the output? Rewrite the extras as commas, colons, or separate sentences.
   - BEFORE: "The team was small -- just three engineers -- but they shipped fast."
   - AFTER: "The team was small. Just three engineers. But they shipped fast."

3. **"Not just...but" constructions:** Find and rewrite as two plain statements.
   - BEFORE: "It's not just about the technology, but about the people behind it."
   - AFTER: "The technology matters. The people behind it matter more."

4. **Dangling -ing clauses:** Check the last 5-8 words of every sentence. If it ends with a vague "-ing" phrase, delete it or rewrite.
   - BEFORE: "The team launched the product, showcasing their commitment to excellence."
   - AFTER: "The team launched the product."

5. **Paragraph openers:** Does any paragraph start with "Additionally," "Furthermore," "Moreover," "Notably," or "Consequently"? Replace with a concrete subject.
   - BEFORE: "Furthermore, the team improved response times."
   - AFTER: "Response times dropped by 40%."

6. **Rule of three:** Look for "X, Y, and Z" patterns. Are they filler? Break them or cut to one strong item.
   - BEFORE: "She brought creativity, dedication, and passion to the role."
   - AFTER: "She redesigned the onboarding flow in her first week."

7. **Puffery:** Is any sentence inflating importance beyond what the facts support? Cut the inflation, keep the facts.
   - BEFORE: "This groundbreaking initiative revolutionized the way teams collaborate."
   - AFTER: "The new tool cut meeting time by half."

8. **Read-aloud test:** Read the output as if speaking it to someone across a table. Flag any sentence that sounds like a press release, a Wikipedia article, or a ChatGPT response. Rewrite those.
   - BEFORE: "The company has established itself as a leader in the rapidly evolving AI landscape."
   - AFTER: "The company ships AI tools that people actually use."

9. **Sentence length variation:** Does the piece have real rhythm variation? If most sentences are roughly the same length (e.g., ten 15-word sentences in a row), break the pattern. Short fragment clusters are fine.
   - BEFORE: "The system processes requests in real time. The architecture supports horizontal scaling. The team monitors performance around the clock."
   - AFTER: "The system processes requests in real time. Scales horizontally. The team watches performance around the clock, though most nights nothing breaks."

10. **Positivity check:** Is the tone more optimistic than the facts warrant? If something was hard, messy, or mixed, does the text say so? If not, add the honest version.
    - BEFORE: "The migration presented challenges but ultimately strengthened the team's capabilities."
    - AFTER: "The migration took three weeks longer than planned. We broke prod twice. But the new system is faster."

11. **Engagement check:** Does the output contain at least one question, first-person reference, or direct address to the reader (where appropriate for the format)? If it's all third-person declarative statements, add a human touch.
    - BEFORE: "The product serves users in 12 countries. Adoption has increased steadily."
    - AFTER: "We're in 12 countries now. Adoption keeps climbing. Honestly, we didn't expect Southeast Asia to take off the way it did."

12. **Formality check:** Does the register match the task? A casual email shouldn't read like a white paper. A formal proposal shouldn't read like a text message. Check for missing contractions in casual contexts and missing precision in formal ones.
    - BEFORE (casual email): "I would like to express my interest in discussing potential collaboration opportunities."
    - AFTER: "I'd love to chat about working together. Free next week?"

13. **Opener check:** Does the piece start with a specific moment, scene, or fact? Or with an abstract statement? Fix if abstract.
    - BEFORE: "In today's fast-paced world, effective communication is more important than ever."
    - AFTER: "Last Tuesday, I sent an email that got a reply in four minutes."

---

## PART 4: QUICK SUBSTITUTION REFERENCE

When you catch yourself reaching for an AI word, swap it:

| Instead of... | Write... |
|---|---|
| delve into | dig into, look at, explore |
| leverage | use |
| foster | build, grow, create |
| facilitate | help, run, set up |
| enhance | improve, strengthen |
| comprehensive | thorough, full, detailed |
| innovative | new, different, original |
| robust | strong, solid |
| landscape (abstract) | space, field, world |
| pivotal | important, big |
| underscore | show, prove, make clear |
| garner | get, earn, win |
| showcase | show, demonstrate |
| bolster | strengthen, support |
| encompass | include, cover |
| cultivate | build, grow |
| navigate (abstract) | handle, manage, work through |
| spearhead | lead, start, run |
| passionate about | care about, drawn to, excited by |
| drives me | motivates me, keeps me going |
| resonates with | matters to, connects to |
| aligns with | matches, fits |
| serves as | is |
| stands as | is |
| plays a crucial role | matters, is important |
| realm | space, area, world |
| notably | (delete, or start with the fact itself) |
| it can be argued | I think, I suspect |
| one may consider | consider, try |
| furthermore | (delete, start with subject) |
| additionally | (delete, start with subject) |
| firstly | first |

---

## Usage Note

This skill is a style filter, not a content generator. It should be applied on top of any writing produced by other skills or prompts. The other skill handles structure, content selection, and strategy. This skill handles voice.

When in doubt, read the sentence out loud and ask: "Would I actually say this to a person sitting across from me?" If no, rewrite it until the answer is yes.
