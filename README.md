# Elastic Documentation Guidelines for LLM

This repository contains all the guidelines, templates, and instructions needed to generate high-quality Elastic-style documentation using Language Models.

## 📁 Repository Structure

```
.
├── README.md                          # This file
├── SYSTEM_PROMPT.md                  # Complete system prompt for LLMs
├── QUICK_START.md                    # Quick start guide
├── guidelines/
│   ├── content-types.md              # Content type guidelines
│   ├── formatting.md                 # Formatting rules
│   ├── style-tone.md                 # Voice, tone, and style
│   ├── grammar-spelling.md           # Grammar and spelling
│   ├── word-choice.md                # Word choice reference
│   └── best-practices.md             # General best practices
├── templates/
│   ├── how-to-template.md            # How-to guide template
│   ├── overview-template.md          # Overview template
│   ├── tutorial-template.md          # Tutorial template
│   ├── troubleshooting-template.md   # Troubleshooting template
│   └── changelog-template.md         # Changelog template
├── prompts/
│   ├── system-prompt-base.txt        # Base system prompt
│   ├── how-to-prompt.txt             # How-to specific prompt
│   ├── overview-prompt.txt           # Overview specific prompt
│   ├── tutorial-prompt.txt           # Tutorial specific prompt
│   ├── troubleshooting-prompt.txt    # Troubleshooting specific prompt
│   └── review-prompt.txt             # Content review prompt
└── examples/
    ├── good-how-to.md                # Example of well-structured how-to
    ├── good-overview.md              # Example of well-structured overview
    └── review-checklist.md           # Quality checklist
```

## 🚀 Quick Start

1. **Copy the system prompt**: See `SYSTEM_PROMPT.md`
2. **Choose your content type**: See `guidelines/content-types.md`
3. **Use the appropriate template**: See `templates/` folder
4. **Follow the specific prompt**: See `prompts/` folder
5. **Review the result**: Use `examples/review-checklist.md`

## 📖 How to Use These Guidelines

### With Claude / ChatGPT / Copilot

```
[Paste SYSTEM_PROMPT.md content into system message]

User message:
"Create a how-to guide about [topic].

Template: [Paste from templates/how-to-template.md]

Guidelines: [Paste from guidelines/]

Create the guide following these rules."
```

### With LLM APIs (OpenAI, Anthropic, Gemini)

See `prompts/` folder for ready-to-use JSON-formatted prompts.

## 📚 Content Types Covered

- **How-to Guides**: Step-by-step instructions for specific tasks
- **Overviews**: Conceptual explanations of features or concepts
- **Tutorials**: Learning-focused, progressive guides
- **Troubleshooting**: Problem identification and resolution
- **Changelogs**: Release notes and version information

## ✅ Quality Assurance

Each generated document should:
- ✓ Match the content type structure
- ✓ Follow formatting and style guidelines
- ✓ Use appropriate tone for the context
- ✓ Use consistent word choice
- ✓ Be accessible and scannable
- ✓ Include relevant examples and links

See `examples/review-checklist.md` for detailed quality criteria.

## 📝 Files Included

| File | Purpose |
|------|----------|
| SYSTEM_PROMPT.md | Complete, ready-to-use system prompt |
| QUICK_START.md | Step-by-step quick start guide |
| guidelines/ | Reference documentation for all aspects |
| templates/ | Markdown templates for each content type |
| prompts/ | LLM-specific prompt formats |
| examples/ | Real examples and checklists |

## 🔍 Key Rules at a Glance

### Tone & Voice
- Professional, plainspoken, direct
- User-focused (use "you")
- Clear and brief
- Active voice
- No fluff or filler

### Style
- American English
- Present tense
- Prefer action verbs
- Use monospace for commands/code
- Use bold for UI elements
- Numbered lists for procedures
- Tables for structured data

### Word Choice
✓ Prefer: create, add, remove, delete, select, enter, open, view, use
✗ Avoid: easy, simply, click (when not mouse), launch, execute

### Structure
- Every content type has a specific required structure
- Headings organize content into a logical hierarchy
- Short paragraphs and scannable lists
- Clear introductions and summaries

## 💡 Tips for Best Results

1. **Start with a clear topic**: "Create a how-to about X"
2. **Specify the audience**: "For beginners / intermediate users"
3. **Use the template**: Always provide the relevant template
4. **Include context**: What product/feature are you documenting?
5. **Review the output**: Use the checklist before publishing

## 📖 Learn More

For complete details, see:
- Content types: `guidelines/content-types.md`
- All style rules: `guidelines/` folder
- Real examples: `examples/` folder

## 📄 License

Based on [Elastic Documentation Guidelines](https://github.com/elastic/docs-content).

---

**Happy documenting! 📚**
