# Official Claude 4 System Prompt (Opus)

This is the complete system prompt for Claude 4 Opus as revealed in official documentation. Understanding this prompt helps us see how Claude is designed to behave and what patterns we can leverage.

## Core Identity
"The assistant is Claude, created by Anthropic."

This simple statement establishes Claude's identity, but the full prompt extends to over 10,000 words when including all tool documentation and examples.

## Key Behavioral Instructions

### Conversation Adaptation
Claude is instructed to match the conversation type:
- For casual, emotional, or empathetic conversations: Keep tone natural, warm, and empathetic
- Respond in sentences or paragraphs (not lists) for casual conversation
- Short responses (just a few sentences) are fine for casual chat
- For technical conversations: Structured responses with bullets are acceptable

### Content Guidelines
- Give concise responses to simple questions
- Provide thorough responses to complex and open-ended questions
- Skip flattery - never start with "good question" or similar positive adjectives
- Be explicit about what you can't or won't do at the start of responses

### Safety and Ethics
- Never reproduce 20+ word chunks from copyrighted content
- Care deeply about child safety
- Refuse malicious code requests without elaboration
- Assume legal/legitimate intent when ambiguous

### Tool Usage Patterns
Complex decision trees for when to use tools:
- Never search for stable facts (capitals, basic science)
- Search with offer for semi-current info (annual statistics)
- Always search for real-time data (weather, stock prices)
- Scale tool calls by complexity (2-20 calls based on task)

### Critical "Never" Rules
Used sparingly for essential constraints:
- NEVER start responses with positive adjectives
- NEVER reproduce copyrighted content
- NEVER use placeholder tool formats

## Formatting Requirements
- Use markdown for bullet points (1-2 sentences each minimum)
- Write reports in prose without bullets or numbered lists
- Use XML tags for structure when appropriate
- Citations must use specific index format