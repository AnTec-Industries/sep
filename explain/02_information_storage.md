# Information Storage Path

## What It Is
The direct path of working with SEP - storing information and getting verification through needed context.

## How It Works
1. Ask "What are you working on?"
2. SEP shows needed context through needed.json:
   ```json
   "content": {
     "tracks": {
       "needed": ["official_track_list", "mod_compatibility"],
       "relevance": "When working with track delivery",
       "current": {
         "status": "have basic structure"
       }
     }
   }
   ```
3. Store the information
4. SEP verifies through showing needed context is met

## Example Flow
1. Working on tracks:
   - Ask "What are you working on?"
   - SEP shows it needs track list and compatibility
   - Store those details
   - SEP verifies by showing context is complete

2. Working on servers:
   - Ask "What are you working on?"
   - SEP shows it needs port range and IPs
   - Store that information
   - SEP verifies through context

## Key Insight
This path shows SEP's direct nature:
1. Ask what it's working on
2. It shows what it needs
3. Provide that
4. It verifies through context

No complexity needed - just ask and respond to context needs.
