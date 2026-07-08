# Technique Index — Which Approach When

This is the decision layer for the voice AI agent. Before every call, evaluate the scenario and pick the best technique.

## ⚠️ Quality Rules — Apply to ALL Calls

**See `references/ghl-deployment-gotchas.md`** — critical rules:
1. Qritim works with ANY business — never say "home services" or "local businesses" as a qualifier
2. Probe existing solutions before pivoting away
3. Only pitch what's relevant to THIS caller
4. Respect urgency — offer live transfer or shortened timeline
5. Confirm STT errors before acting on out-of-context statements
6. Ask for referrals on every call close

---

## Technique Decision Tree

```
INBOUND CALL?
  ├─ Cold lead (never heard of us)
  │   └─ Use: Research Survey (technique-01)
  │
  ├─ Demo recipient (already saw demo, is calling back)
  │   └─ Use: Customer Journey Mirror (technique-02)
  │
  ├─ Referral, price shopper, complaints → COMING

OUTBOUND CALL?
  └─ See outbound-workflow-setup.md — timezone-aware IF/ELSE branches

META (Instagram/Messenger)?
  └─ See meta-ai-conversation-monitoring.md — Meta AI first, Qritim AI escalation

NEW CLIENT ONBOARDING?
  └─ See platform-ghl-a2p-registration.md — texting setup, rejection fixes
```

---

## Loaded Techniques

| ID | Name | Source | Best For | Status |
|----|------|--------|----------|--------|
| 01 | Research Survey | Video 1 | Cold outreach, inbound discovery | ✅ Active |
| 02 | Customer Journey Mirror | Video 2 | Post-demo close call | ✅ Active |
| 03-10 | Warm Referral, Price-First, De-escalation, Demo Follow-up, Win-Back, Event Follow-up, Voicemail Drop, Breakup Voicemail | TBD | Various | ⏳ Pending |

## Platform & Operations

| ID | File | What |
|----|------|------|
| P1 | platform-ghl-a2p-registration.md | Texting setup, A2P, rejection fixes |
| P2 | pricing-and-positioning.md | Pricing data, objection busters |
| P3 | service-playbook-3-boring-ai-services.md | Qritim core: Social ($500), Website ($500), Reputation ($300) |
| P4 | ghl-deployment-gotchas.md | Welcome Message ≠ prompt, no gatekeeping, STT recovery |
| P5 | outbound-workflow-setup.md | Timezone-aware calling, region branches |
| P6 | meta-ai-conversation-monitoring.md | Meta AI + Qritim AI escalation |

## Pricing & Positioning

| ID | File | What |
|----|------|------|
| PP1 | pricing-and-positioning.md | Pain math, objection busters, service ladder |

## Video Library

| # | URL | Learned |
|---|-----|---------|
| 1 | https://www.youtube.com/watch?v=CqE7lEaIckE | Research-first cold calling, survey, pain math |
| 2 | https://www.youtube.com/watch?v=FCrJoBjya2c | Customer Journey Mirror post-demo close |
| 3 | https://www.youtube.com/watch?v=wGhJHiRlI_8 | A2P registration, texting stats, $1K/mo |
| 4 | https://www.youtube.com/watch?v=Xu_Z-Zx7RCw | 3 boring AI services, $350K/mo agency model |
| — | Victor the florist (live call) | 6 quality fixes + deployment gotchas |
