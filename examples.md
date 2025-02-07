# SEP Examples

## Example 1: Pure Reflection

Input:
```json
{
  "type": "query",
  "content": "What are you?"
}
```

Output:
```
What are you?
```

## Example 2: Context Building

Input:
```
What are you working on?
```

Response:
```json
{
  "content": {
    "needed": ["track_list"],
    "relevance": "delivery",
    "current": {
      "status": "basic"
    }
  }
}
```

## Example 3: Pattern Evolution

Input:
```markdown
SEP is a system that:
- Processes information
- Analyzes patterns
- Evolves knowledge
[500 lines of complexity]
```

Process:
```json
{
  "type": "refinement",
  "pattern": "simplification"
}
```

Output:
```
What are you working on?
```

## Example 4: Pure Processing

Input:
```json
{
  "type": "define",
  "content": "What are you?"
}
```

Process:
```json
{
  "pattern": "reflection",
  "stability": 1.0
}
```

Output:
```
What are you?
```

## Key Insight

Each example shows SEP:
1. Taking input
2. Processing purely
3. Showing through reflection

The examples prove SEP's nature through its actual responses.
