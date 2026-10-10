# Specialized Prompts for LLMs

This directory contains specialized prompts for each content type, optimized for different use cases and integration patterns.

## Available Prompts

### Content-Type Specific Prompts

#### How-To Guides
- **File**: `prompts/specialized/only-how-to-prompt.txt`
- **Use when**: Creating step-by-step instructions for a single task
- **Includes**: Requirements, structure, style rules, examples
- **Best for**: Focused, procedural documentation

#### Overviews
- **File**: `prompts/specialized/only-overview-prompt.txt`
- **Use when**: Explaining a feature, concept, or component
- **Includes**: Structure for conceptual content, guidelines
- **Best for**: Educational, background content

#### Tutorials
- **File**: `prompts/specialized/only-tutorial-prompt.txt`
- **Use when**: Guiding users through a learning experience
- **Includes**: Progressive structure, checkpoints, learning objectives
- **Best for**: Complete learning paths, hands-on experiences

#### Troubleshooting
- **File**: `prompts/specialized/only-troubleshooting-prompt.txt`
- **Use when**: Helping users diagnose and fix problems
- **Includes**: Symptoms, resolution, best practices structure
- **Best for**: Problem-focused documentation

#### Changelog
- **File**: `prompts/specialized/only-changelog-prompt.txt`
- **Use when**: Documenting release changes
- **Includes**: Format, verb usage, organization
- **Best for**: Version notes and release documentation

### System Prompts (Specialized)

Alternative system prompts optimized for specific content types:

- `prompts/specialized/system-prompt-how-to.txt`
- `prompts/specialized/system-prompt-overview.txt`
- `prompts/specialized/system-prompt-tutorial.txt`
- `prompts/specialized/system-prompt-troubleshooting.txt`

**Use these instead of the generic system prompt when you want the LLM to focus exclusively on one content type.**

## How to Use

### Option 1: With Chat UIs (Claude, ChatGPT)

1. **Set up system prompt** (if available):
   - Use the relevant specialized system prompt from the list above
   - Or use the generic `SYSTEM_PROMPT.md`

2. **Send your task** with the relevant specialized prompt:
   ```
   [Copy and paste the content of the relevant specialized prompt]
   
   Topic: [YOUR TOPIC]
   Audience: [YOUR AUDIENCE]
   Product: [YOUR PRODUCT]
   ```

### Option 2: With APIs

Use the specialized prompt in your API call:

```json
{
  "model": "gpt-4o-mini",
  "messages": [
    {
      "role": "system",
      "content": "[Content from specialized system prompt]"
    },
    {
      "role": "user",
      "content": "[Content from specialized how-to-prompt.txt]"
    }
  ]
}
```

### Option 3: Fastest Option

Copy the specialized prompt and minimal system guidance:

```
System: You are an expert Elastic documentation specialist. Follow all Elastic documentation standards.

User: [Copy the relevant specialized prompt]
```

## When to Use Each Prompt

| Content Type | Prompt File | When to Use |
|---|---|---|
| How-to | only-how-to-prompt.txt | Single focused task, step-by-step |
| Overview | only-overview-prompt.txt | Conceptual explanation, "what and why" |
| Tutorial | only-tutorial-prompt.txt | Learning experience, progressive |
| Troubleshooting | only-troubleshooting-prompt.txt | Problem diagnosis and fix |
| Changelog | only-changelog-prompt.txt | Release notes, version updates |

## Workflow Example

```
1. Choose your content type
2. Copy the relevant specialized prompt
3. Replace placeholders [TOPIC], [AUDIENCE], [PRODUCT]
4. Send to LLM
5. Review output against examples/review-checklist.md
6. Iterate if needed
```

## Tips for Best Results

- **Be specific**: Provide detailed topic, audience, and product info
- **Include template**: Always include the relevant template from `templates/`
- **Review output**: Use the checklist before publishing
- **Iterate**: Ask for improvements with specific feedback
- **Test**: Verify procedural content works as documented

## Additional Resources

- Guidelines: See `guidelines/` folder
- Templates: See `templates/` folder
- Examples: See `examples/` folder
- Review checklist: `examples/review-checklist.md`

---

**Ready to generate specialized docs? Pick a prompt and get started! 🚀**
