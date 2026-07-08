# GHL Voice AI Deployment Gotchas

Hard-won lessons from live deployment. Read before pasting any prompt into GHL.

---

## Pitfall 1: Welcome Message Is a SEPARATE Field

The system prompt is NOT the first thing the caller hears. GHL Voice AI has a **Welcome Message** field in the agent settings that fires before the prompt. If it says "I help home service businesses..." that's what they hear — no matter what your prompt says.

**Fix:** Update BOTH the system prompt AND the Welcome Message. The Welcome Message should match the opening line in Step 1 of the prompt.

---

## Pitfall 2: "Local Businesses" Gatekeeps Callers

Every time "local businesses" or "home services" appears in your opening, you lose non-service-business callers. Qritim is a full AI marketing agency — med spas, flower shops, consultancies, education, retail, law firms, everything. The prompt must NEVER say "we mainly focus on" or "we mostly work with" — it makes callers feel like exceptions.

**Rule:** The words "local businesses" and "home service" should appear ZERO times in the opening and Role sections.

---

## Pitfall 3: "We'll call you back" Loses Urgent Leads

When a caller says "I should be talking to someone right now" — offer live escalation, not a callback. If live transfer isn't available, shorten to same-day.

**Fix:** The prompt must have an escalation path: "Let me see if I can get someone on the line right now. If not, within the hour."

---

## Pitfall 4: STT Hallucinations Look Like Real Problems

"I'm free in the evening" transcribed as "I'm feeling dizzy" → agent launches health concern script. Before acting on ANY out-of-context statement, confirm: "Just to confirm — did you say [best guess]?"

---

## Pitfall 5: Outbound Time Window Is Per-Workflow, Not Per-Contact

GHL's time window setting applies globally to the workflow. If your account is in Nepal (NPT) and you set 8AM-5PM, you're calling US businesses at 10PM-7AM. 

**Fix:** Use IF/ELSE branches based on a "Target Region" custom field. Each branch has its own time logic. See `references/outbound-workflow-setup.md`.

---

## Pitfall 6: The Prompt Must Use GHL Custom Values

GHL expects `{{contact.first_name}}`, `{{contact.last_name}}`, `{{contact.email}}`, `{{contact.phone}}` in the prompt. Plain text like "[first name]" won't resolve. The prompt structure must follow GHL's expected format with `# Role and Identity`, `# Speaking Style`, `# Call Flow` sections.
