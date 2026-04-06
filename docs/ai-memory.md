# How AI memory works

### The context window, is working memory
- system prompt
- Conversation history
- Retrieved documents
- User input

## The AI memory hierarchy

1. model weights, like ROM (Read Only Memory) / Firmware:

- 175B parameters
- Compressed knowledge
- Cannot change at runtime

2. system prompt, like BIOS settings

3. retrieved context, like loading from disk into RAM
- vector databases
- documents
- APIs

4. Persistent memory, like user profile storage
- user preferences
- past interactions
- selectively loaded based on relevance

its not too different from the traditional computer memory hierarchy:

| Traditional | AI / LLM |
| --- | --- |
| Registers: fast, tiny | Weights: fixed, compressed |
| Cache: fast, small | Context: fast, limited |
| RAM: medium | Retrieved: dynamic, selective |
| Disk: slow, large | Memory: slow, persistent |



