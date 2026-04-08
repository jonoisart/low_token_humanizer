---
name: low_token_humanizer
version: 1.0.0
description: Compressed reference for removing AI writing patterns. Derived from blader/humanizer.
license: MIT
---
# low_token_humanizer

This version strips everything except the pattern rules, making it small enough to embed directly in CLAUDE.md or AGENTS.md without meaningfully impacting context budgets.

### Option 1: Clone the repo

```bash
git clone https://github.com/di3italis/low_token_humanizer.git
```

Then copy the contents of `low_token_humanizer.md` into your agent's global instruction file (see Adding to your agent below).

### Option 2: Copy and paste

Open `low_token_humanizer.md` in GitHub, select all, and paste the contents directly into your agent instruction file or prompt.

---

## Adding to your agent

Depending on your tool, the global instruction file may be called `CLAUDE.md`, `AGENTS.md`, `.cursorrules`, `system_prompt.md`, or similar. It's the file your agent reads at startup to understand how it should behave.

**If you're not sure where that file is**, paste the contents of `humanizer-compact.md` into a conversation with your agent and say:

> Add this to your global instruction file.

The agent will handle the rest.

---

## Usage

Once the rules are in your agent's global instruction file, no invocation is needed — the patterns will be applied automatically to all responses.

To humanize a specific piece of text on demand:

> Humanize this: [paste text]

To match your own writing style, include a sample:

> Humanize this: [paste text]. Match the voice in this sample: [paste sample]

The agent will automatically flag any remaining AI patterns after the first pass and revise before returning the final output.

---

## Full example

### Before

> The integration of artificial intelligence and human ingenuity offers a transformative pathway to address the existential threats of war, famine, and environmental collapse by creating a symbiotic partnership where AI handles computational heavy lifting and humans provide strategic foresight, ethical grounding, and empathy. By leveraging AI's unparalleled capacity for real-time data analysis, we can detect early warning signs of conflict, predict crop failures, and model complex climate scenarios, enabling a shift from reactive crisis management to proactive prevention. However, the true power lies in using these tools as force multipliers for human judgment, where AI optimizes resource distribution, monitors environmental changes, and simulates policy outcomes, while humans define the goals of justice and sustainability and ensure solutions remain equitable. Ultimately, establishing robust governance frameworks to prevent bias and ensure global benefit will allow this collaboration to build a future where technological speed and scale serve as the bedrock for lasting peace, food security, and ecological restoration.

### After

> Artificial intelligence isn't just a tool for efficiency; it's a force multiplier for human intuition when tackling global crises like famine, war, or environmental collapse. While algorithms can process massive datasets to predict crop failures or track deforestation in real time, the final decisions on where to send help still require local knowledge and political will. The real breakthrough happens when AI handles the heavy lifting of data synthesis while humans focus on strategy and empathy — interpreting simulations, understanding cultural nuances, and mobilizing community trust. Ultimately, course-correcting requires a feedback loop where technology optimizes supply chains and models climate scenarios, but human oversight prevents bias and ensures fairness. When a disaster strikes, an algorithm might identify the most efficient rescue route, but it is the human team on the ground who decide who gets saved first and how to comfort survivors. The goal isn't to build a self-piloting civilization, but to create a hybrid system where machines expand our capacity to act and humans provide the purpose behind those actions.

---

## Reference

Based on [blader/humanizer](https://github.com/blader/humanizer), which is in turn based on [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), maintained by WikiProject AI Cleanup. The patterns documented there come from observations of thousands of instances of AI-generated text on Wikipedia.

---

## Version history

- **1.0.0** — Initial release

---

## License

MIT
