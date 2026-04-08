# low_token_humanizer

A token-minimized reference derived from [blader/humanizer](https://github.com/blader/humanizer).

This version strips everything except the pattern rules, making it small enough to embed directly in `CLAUDE.md` or `AGENTS.md` without meaningfully impacting context budgets.

The original is a full Claude Code skill with examples, voice calibration walkthroughs, and process scaffolding — well-suited for standalone use. 

Use the original if you want the full skill with examples and voice matching. Use this if you need the rules inline and always-on.

## Full Example
### Before
The integration of artificial intelligence and human ingenuity offers a transformative pathway to address the existential threats of war, famine, and environmental collapse by creating a symbiotic partnership where AI handles computational heavy lifting and humans provide strategic foresight, ethical grounding, and empathy. By leveraging AI's unparalleled capacity for real-time data analysis, we can detect early warning signs of conflict, predict crop failures, and model complex climate scenarios, enabling a shift from reactive crisis management to proactive prevention. However, the true power lies in using these tools as force multipliers for human judgment, where AI optimizes resource distribution, monitors environmental changes, and simulates policy outcomes, while humans define the goals of justice and sustainability and ensure solutions remain equitable. Ultimately, establishing robust governance frameworks to prevent bias and ensure global benefit will allow this collaboration to build a future where technological speed and scale serve as the bedrock for lasting peace, food security, and ecological restoration.

### After
Artificial intelligence isn't just a tool for efficiency; it's a force multiplier for human intuition when tackling global crises like famine, war, or environmental collapse. While algorithms can process massive datasets to predict crop failures or track deforestation in real time, the final decisions on where to send help still require local knowledge and political will. The real breakthrough happens when AI handles the heavy lifting of data synthesis while humans focus on strategy and empathy—interpreting simulations, understanding cultural nuances, and mobilizing community trust. Ultimately, course-correcting requires a feedback loop where technology optimizes supply chains and models climate scenarios, but human oversight prevents bias and ensures fairness. When a disaster strikes, an algorithm might identify the most efficient rescue route, but it is the human team on the ground who decide who gets saved first and how to comfort survivors. The goal isn't to build a self-piloting civilization, but to create a hybrid system where machines expand our capacity to act and humans provide the purpose behind those actions.

## Reference

This skill is based on https://github.com/blader/humanizer, which in turn is based on [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), maintained by WikiProject AI Cleanup. The patterns documented there come from observations of thousands of instances of AI-generated text on Wikipedia.

## Version History

- **1.0.0** - Initial release

## License

MIT
