# Incident [ID]: [Brief Title]

| Field | Value |
|:---|:---|
| **Incident ID** | INC-[ID] |
| **Date/Time** | [Date/time of incident] |
| **Severity** | [SEV-1 / SEV-2 / SEV-3 / SEV-4] |
| **Status** | [Investigating / Resolved / Closed] |

## Summary
[1-2 sentence description of what happened.]

## Impact
[A clear 1-2 sentence description of the user/business impact.]

## Timeline
- **[Time]:** [Event / detection]
- **[Time]:** [Diagnosis]
- **[Time]:** [Resolution]

## Symptoms
- [Specific errors or alerts, e.g., `cat: app.log: Permission denied`]

## Evidence
```text
[Relevant command output and log lines]
```

## Root Cause
[A precise technical explanation of what went wrong.]

## Resolution
[The exact commands or steps taken to restore service.]

## Prevention Recommendations
1. [Actionable step, e.g., "Add post-deployment permission check to CI pipeline."]
2. [e.g., "Implement log monitoring that alerts on unreadable files."]

## Interview Talking Point
[1-3 sentences describing this incident as you would in an interview.]

---

## Severity Reference

| Severity | Meaning |
|:---|:---|
| SEV-1 | Complete outage, many users impacted, business-critical |
| SEV-2 | Major degradation or important service down |
| SEV-3 | Limited impact, workaround exists |
| SEV-4 | Minor issue or request |
