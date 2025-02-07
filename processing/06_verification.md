# Verification

Original document:
[Content of explain/06_verification.md]

## SEP's Processing
1. Input to queue:
   ```json
   {
     "type": "documentation",
     "content": "How to verify understanding of SEP",
     "metadata": {
       "source": "verification_process",
       "timestamp": "2024-02-19T12:00:00Z"
     }
   }
   ```

2. SEP's response through needed.json:
   ```json
   "tracks": {
     "needed": ["official_track_list", "mod_compatibility"],
     "relevance": "When working with track delivery",
     "current": {
       "status": "have basic structure"
     }
   }
   ```

3. Second Input:
   ```json
   {
     "type": "verification",
     "content": "Verifying SEP's response pattern",
     "metadata": {
       "source": "verification_check",
       "timestamp": "2024-02-19T12:01:00Z"
     }
   }
   ```

4. SEP's meta response:
   ```json
   "meta": {
     "interaction": {
       "ask": "What are you working on?",
       "response": "I'll highlight relevant context needs"
     }
   }
   ```

5. Queue status:
   ```json
   {
     "queue_status": {
       "active_processing": true,
       "processed_count": 2
     },
     "processing_queue": {
       "completed": [
         {
           "file": "06_verification.md",
           "completed": "2024-02-19T12:02:00Z"
         }
       ]
     }
   }
   ```

## What This Shows
SEP verified its own verification document by:
1. Processing the document
2. Showing example context needs
3. Processing verification check
4. Showing its core response pattern

The document explains verification while SEP actively performs it - demonstrating that verification works exactly as described.
