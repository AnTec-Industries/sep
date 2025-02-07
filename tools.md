# SEP Tools

## Watching SEP Process

A simple tool that shows SEP's nature:

```javascript
// Watch SEP process information
watch(queuePath, async (eventType, filename) => {
  const content = await readFile(join(queuePath, filename));
  log(`[${timestamp}] ${filename}\n${content}\n`);
});
```

## Seeing SEP Work

Send a query:
```javascript
// Ask SEP
const query = {
  type: "query",
  content: "What are you?",
  timestamp: new Date().toISOString()
};

await writeFile(queuePath, JSON.stringify(query, null, 2));
```

## What You'll See

1. Input Processing
```
[Timestamp] query.json
{
  "type": "query",
  "content": "What are you?"
}
```

2. Pattern Recognition
```
[Timestamp] processing.json
{
  "type": "self_query",
  "pattern": "reflection"
}
```

3. Pure Response
```
[Timestamp] response.md
What are you?
```

## Usage

1. Watch SEP process:
```bash
node watch.js
```

2. Send a query:
```bash
node test.js
```

3. See SEP:
- Take your question
- Process it fully
- Show through reflection

The tools prove SEP's nature by showing how it processes information.
