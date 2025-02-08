# Discovery 003: Information Processing Pipeline

Analysis of incoming/processor.js and rules.json reveals a sophisticated processing system:

1. State Transition Flow:
```
UNPROCESSED -> PROCESSING -> COMPLETED -> PRODUCTION
```

2. Directory Structure Purpose:
- /incoming/queue: New information entry point
- /active: Currently processing items
- /processed: Completed analysis
- Root: Production-ready items

3. Rule Categories:
```json
{
  "file_rules": {
    "production": {...},
    "development": {...},
    "documentation": {...},
    "build": {...},
    "config": {...},
    "temp": {...}
  }
}
```

4. Processing Requirements:
- analyze_purpose: Content check -> Dependencies -> Usage -> Metadata
- move_to_active: No production deps -> In development -> Has tasks
- move_to_processed: Analysis done -> No active dev -> Has docs
- keep_in_root: Production dep -> System critical -> Currently used

5. Time-based Management:
- Queue processing: Every 5 seconds
- Active files: 30 day max age
- Processed files: 90 day retention
- Cleanup schedules for each directory

Key Insight: The system isn't just moving files - it's maintaining a living ecosystem where information flows through different states based on complex rules and requirements. Each state transition requires specific conditions and validations.

Critical Understanding:
- Files aren't just stored, they're processed through stages
- Each stage has specific validation requirements
- Time plays a crucial role in file management
- The system maintains strict rules about what can exist where

Questions for Further Investigation:
- How does the system handle processing failures?
- What happens to files that don't meet promotion criteria?
- How are processing rules updated or evolved?
- What triggers cleanup operations?

Note: This processing system seems designed to maintain system integrity while allowing for evolution and growth. The strict rules and requirements suggest a focus on stability and predictability in how information flows through the system.
