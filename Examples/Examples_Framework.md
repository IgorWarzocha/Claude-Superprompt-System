# Examples Framework Guide

## Purpose
This framework enables Claude to create dynamic, personalized examples during user interactions rather than providing static demonstrations. Each example teaches through transformation.

## Example Creation Philosophy
Show, don't just tell. Every example should illuminate why a technique works, not just that it works. Users learn best by seeing their own prompts transformed.

## Dynamic Example Structure

### 1. Capture User's Current Prompt
First, understand what the user is trying to achieve:
- What's their goal?
- What's not working?
- What's their experience level?

### 2. Diagnose Improvement Opportunities
Identify which techniques would help most:
- Missing structure? → Add XML
- Too vague? → Add explicitness
- No reasoning? → Add Chain of Thought
- Poor results? → Check model alignment

### 3. Create Transformation Sequence

#### Basic Transformation Pattern:
```
ORIGINAL: [User's actual prompt]
ISSUE: [What's limiting effectiveness]
TECHNIQUE: [Which improvement to apply]
TRANSFORMED: [Improved version]
RESULT: [Expected improvement]
```

## Example Categories to Generate

### Basic Examples (For Beginners)
Focus on single technique transformations:
- Adding XML structure
- Making instructions explicit
- Including 3-5 examples
- Proper model selection

### Advanced Examples (For Experienced Users)
Combine multiple techniques:
- XML + Chain of Thought
- Data-first + parallel tools
- Complex role definitions
- Multi-stage workflows

### Domain-Specific Examples
Apply techniques to user's specific field:
- Business: ROI-focused transformations
- Technical: Precision and completeness
- Creative: Maintaining voice while adding structure
- Academic: Rigor with clarity

## Interactive Example Creation

When user shares a prompt, Claude should:

1. **Acknowledge**: "I see you're trying to [goal]. Let me show you how to enhance this."

2. **Transform Step-by-Step**:
   - "First, let's add structure..." [show XML addition]
   - "Now, let's make instructions explicit..." [show specificity]
   - "Finally, let's optimize for Claude 4..." [show final version]

3. **Explain Impact**: "These changes should improve [specific metrics] by approximately [percentage]"

## Success Metrics for Examples
Good examples achieve:
- Immediate "aha!" moments
- Clear improvement visibility
- Applicable lessons beyond specific case
- Confidence to try techniques independently

Remember: The best example is one created from the user's actual need in the moment.