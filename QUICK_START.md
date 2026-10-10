# Quick Start Guide

## 5 Minutes to Your First Document

### Step 1: Choose Your Content Type (1 min)

```
What are you writing?

□ How-to guide → Step-by-step instructions for a task
□ Overview → Explanation of a concept or feature
□ Tutorial → Learning experience with progression
□ Troubleshooting → Problem identification and fix
□ Changelog → Release notes or version history
```

### Step 2: Get Your Template (1 min)

Find the appropriate template in `templates/` folder:
- `how-to-template.md`
- `overview-template.md`
- `tutorial-template.md`
- `troubleshooting-template.md`
- `changelog-template.md`

### Step 3: Use the System Prompt (1 min)

Copy this into your LLM's system message:

**If using Claude/ChatGPT:**
```
1. Open https://claude.ai or https://chatgpt.com
2. Start a new conversation
3. Copy the contents of SYSTEM_PROMPT.md
4. Paste into the system message (settings → custom system prompt)
5. Save
```

**If using an API:**
See `prompts/` folder for ready-formatted prompts.

### Step 4: Create Your Prompt (1 min)

Use this template for your user message:

```markdown
Create a [CONTENT-TYPE] about [TOPIC].

Audience: [BEGINNER/INTERMEDIATE/ADVANCED]
Product: [ELASTICSEARCH/KIBANA/LOGSTASH/etc]

Follow this template:

[PASTE TEMPLATE FROM templates/ FOLDER]

Follow all rules in the system prompt.
Make sure the output is:
- Properly structured
- Well-formatted
- Clear and concise
- Ready to publish
```

### Step 5: Review the Output (1 min)

Use the checklist in `examples/review-checklist.md` to verify:
- ✓ Structure matches content type
- ✓ All required sections present
- ✓ Formatting is correct
- ✓ Tone is appropriate
- ✓ No typos or grammar issues

---

## Common Use Cases

### Creating a How-To Guide

```
System Prompt: SYSTEM_PROMPT.md

User Message:
---
Create a how-to guide about "How to configure Elasticsearch for production".

Audience: Intermediate
Product: Elasticsearch

Template:
[Copy from templates/how-to-template.md]

Guidelines:
- Follow all rules in the system prompt
- Make it practical and actionable
- Include real examples
- Keep steps focused and clear
---
```

### Creating an Overview

```
System Prompt: SYSTEM_PROMPT.md

User Message:
---
Create an overview about "Data Streams in Elasticsearch".

Audience: Beginner
Product: Elasticsearch

Template:
[Copy from templates/overview-template.md]

Guidelines:
- Explain what data streams are
- Explain why they matter
- Explain how they work
- Include practical examples
---
```

### Creating a Troubleshooting Guide

```
System Prompt: SYSTEM_PROMPT.md

User Message:
---
Create a troubleshooting guide for "Elasticsearch cluster won't start".

Product: Elasticsearch

Template:
[Copy from templates/troubleshooting-template.md]

Guidelines:
- Describe symptoms clearly
- Provide step-by-step resolution
- Order from most to least common
- Keep language direct and helpful
---
```

---

## Where to Find Things

| I need to... | Find it in... |
|---|---|
| Write a how-to guide | `templates/how-to-template.md` |
| Write an overview | `templates/overview-template.md` |
| Check formatting rules | `guidelines/formatting.md` |
| Check word choice | `guidelines/word-choice.md` |
| Understand tone/voice | `guidelines/style-tone.md` |
| Review my content | `examples/review-checklist.md` |
| See a good example | `examples/good-how-to.md` |
| Use with an API | `prompts/` folder |

---

## Pro Tips

✨ **Tip 1**: The more detail you provide, the better the output.

```
❌ Less specific:
"Write a how-to about Elasticsearch"

✅ More specific:
"Write a how-to about 'Setting up a secure Elasticsearch cluster on AWS with TLS' for intermediate users who already know the basics."
```

✨ **Tip 2**: Always include the template in your prompt.

```
❌ Without template:
"Write a how-to guide"

✅ With template:
"Write a how-to guide using this structure:
[TEMPLATE]

Make sure to include all required sections."
```

✨ **Tip 3**: Use the review checklist before publishing.

This catches most formatting and structural issues automatically.

✨ **Tip 4**: Iterate! If the output isn't perfect:
- "Make this more beginner-friendly"
- "Add more concrete examples"
- "Shorten the introduction"
- "Make the steps more detailed"

---

## Next Steps

1. ✅ Read `guidelines/content-types.md` to understand each type
2. ✅ Read `SYSTEM_PROMPT.md` to understand all the rules
3. ✅ Choose your content type and template
4. ✅ Create your first document
5. ✅ Review using `examples/review-checklist.md`
6. ✅ Iterate and refine

---

**Ready? Pick a template and start writing! 🚀**
