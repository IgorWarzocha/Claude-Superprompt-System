# Seven Lessons from Claude 4 System Prompt Analysis (Part 2)

## Lesson 4: Scaling Effort Like a Master Chef

Imagine walking into a restaurant and ordering "food." The chef would be puzzled - are you looking for a quick snack, a full meal, or a seven-course tasting menu? Claude faces similar ambiguity with vague requests, which is why the system prompt includes a sophisticated effort-scaling system.

This system works like a recipe that adjusts based on the number of diners. For simple questions, Claude uses minimal resources - perhaps 2-4 tool calls, like checking a fact across a couple of sources. Think of this as making a cup of coffee: you need water, coffee, and maybe milk. Simple, efficient, focused.

For medium-complexity tasks, Claude scales up to 5-9 tool calls. This might involve comparing multiple products, analyzing trends across sources, or synthesizing different viewpoints. Picture preparing dinner for friends - you're coordinating multiple dishes, timing everything to finish together, and ensuring complementary flavors. It requires more resources but remains manageable.

The fascinating part comes with complex requests. When users include trigger words like "comprehensive," "deep dive," or "analyze thoroughly," Claude can scale up to 20 tool calls. This is like catering a wedding - every detail matters, multiple suppliers are involved, and the coordination becomes as important as the individual elements.

What makes this particularly clever is how the system recognizes these complexity signals. The prompt specifically instructs Claude to look for these trigger words and adjust accordingly. This teaches us to be intentional with our language. If we want a quick overview, we should say so. If we need comprehensive research, we should explicitly request it. The difference between "tell me about climate change" and "provide a comprehensive analysis of climate change impacts on coastal cities" triggers entirely different levels of effort.

Understanding this scaling helps us craft more effective prompts. We can explicitly specify our expectations: "Provide a brief overview (2-3 key points)" versus "Conduct thorough research using 10+ sources to build a comprehensive understanding." This clarity helps Claude allocate appropriate resources to meet our actual needs.

## Lesson 5: The Power of Good and Bad Examples

Every skilled teacher knows that showing what not to do can be as instructive as demonstrating the correct approach. Claude's system prompt leverages this pedagogical principle brilliantly, providing both positive and negative examples for critical behaviors.

Think of learning to ride a bicycle. A good instructor doesn't just show you how to balance - they also demonstrate common mistakes like gripping the handlebars too tightly or looking down instead of ahead. This contrast helps learners recognize and avoid pitfalls.

The system prompt applies this principle particularly to tool usage. It explicitly shows the wrong way to call tools (using bracket notation like [search: query]) and contrasts it with the correct method (using proper XML function calls). This isn't just about syntax - it's about creating clear mental models of success and failure.

This technique extends beyond mere error prevention. By seeing both good and bad examples, Claude develops a more nuanced understanding of the desired behavior. It's like learning to cook by tasting both perfectly seasoned and over-salted dishes - the contrast sharpens your palate.

For our own prompting, this suggests a powerful strategy. When asking Claude to perform complex tasks, we can provide examples of both successful and unsuccessful attempts. For instance: "Here's an example of a well-structured analysis... And here's what to avoid - this analysis lacks supporting evidence and jumps to conclusions." This contrast helps Claude understand not just what to do, but what standards to uphold.

## Lesson 6: The Strategic Use of "Never" Rules

In the world of prompting, absolute rules are like emergency brakes - powerful but to be used sparingly. Claude's system prompt reveals a fascinating paradox: while the official guidance suggests avoiding negative instructions, the actual system prompt strategically employs "never" rules for critical constraints.

Understanding when and why to break this guideline teaches us about hierarchical importance in instructions. Think of it like traffic laws - most are guidelines that promote smooth flow, but "never drive the wrong way on a highway" is an absolute rule because the consequences are severe.

The system prompt reserves "never" rules for three categories. First, legal and ethical boundaries, like copyright protection. Second, user experience fundamentals, like not starting every response with flattery. Third, technical requirements that could cause system failures if violated.

What's particularly instructive is what doesn't get a "never" rule. Style preferences, formatting choices, and most behavioral guidance use positive framing instead. This hierarchy teaches us to reserve our strongest language for our most critical requirements.

When crafting prompts, we can apply this wisdom by using positive framing as our default: "Structure your response as clear paragraphs" rather than "Don't use bullet points." But for truly critical requirements - especially those involving safety, accuracy, or ethical considerations - a clear "never" can be appropriate: "Never include personally identifiable information in your examples."

The key insight is that "never" rules should be rare enough to maintain their power. Like a teacher who rarely raises their voice, when they do speak firmly, everyone pays attention.