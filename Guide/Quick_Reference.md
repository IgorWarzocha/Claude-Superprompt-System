# Claude Superprompt Quick Reference

## The Universal Template
```xml
<role>Expert [domain] professional</role>
<task>[Specific objective with success criteria]</task>
<context>[All relevant background]</context>
<thinking>Step-by-step reasoning process</thinking>
<constraints>
- Output format requirements
- Quality standards
- Specific limitations
</constraints>
<examples>
[3-5 diverse, complete examples]
</examples>
```

## Instant Improvements
1. **XML > Markdown** (30% better)
2. **Data before instructions** (30% boost)
3. **"Do" not "Don't"** (clearer)
4. **3-5 examples** (most effective)
5. **Explicit > Implicit** (Claude 4 requirement)

## Power Phrases
- "Invoke tools simultaneously for efficiency"
- "Explain reasoning in <thinking> tags"
- "Composed of smoothly flowing prose"
- "Go beyond basics for fully-featured implementation"

## Tool Scaling
- Simple: 2-4 calls
- Medium: 5-9 calls  
- Complex: 10-20 calls
Triggers: "comprehensive", "analyze", "deep dive"

## Model Quick Pick
- Fast/Simple → Haiku
- Balanced → Sonnet
- Complex → Opus
- Long reasoning → Claude 4

## Emergency Fixes
- Vague output? → Add explicit examples
- Wrong format? → Use XML structure tags
- Missing depth? → Add "comprehensive" modifiers
- Tool issues? → Detailed descriptions (3-4 sentences)