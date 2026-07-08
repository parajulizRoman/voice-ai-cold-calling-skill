# Technique Index — Which Approach When

This is the decision layer for the voice AI agent. Before every call, evaluate the scenario and pick the best technique.

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
  ├─ Referral ("Mike told me to call")
  │   └─ Use: Warm Referral (technique-03) — COMING
  │
  ├─ Price shopper ("How much does it cost?")
  │   └─ Use: Price-First Qualification (technique-04) — COMING
  │
  ├─ "Texting feels spammy" or "I don't want to text my customers"
  │   └─ Use data from pricing-and-positioning.md: 98% open rate, 45% reply rate
  │
  ├─ "Too expensive" / pricing objection
  │   └─ Use pain math from pricing-and-positioning.md: missed calls × ticket value
  │
  └─ Angry/frustrated ("Your AI called me 3 times!")
      └─ Use: De-escalation (technique-05) — COMING

OUTBOUND CALL?
  ├─ Cold list (no prior contact)
  │   └─ Use: Research Survey (technique-01)
  │
  ├─ Demo sent, no response (follow-up)
  │   └─ Use: Demo Follow-up (technique-06) — COMING
  │
  ├─ Past client (churned or dormant)
  │   └─ Use: Win-Back (technique-07) — COMING
  │
  └─ Event/conference lead
      └─ Use: Event Follow-up (technique-08) — COMING

VOICEMAIL?
  ├─ First attempt
  │   └─ Use: Voicemail Drop (technique-09) — COMING
  │
  └─ Third+ attempt
      └─ Use: Breakup Voicemail (technique-10) — COMING

ONBOARDING A NEW CLIENT?
  └─ See platform-ghl-a2p-registration.md — texting setup, timelines, rejection fixes
```

---

## Loaded Techniques

| ID | Name | Source | Best For | Status |
|----|------|--------|----------|--------|
| 01 | Research Survey | [Video 1](https://www.youtube.com/watch?v=CqE7lEaIckE) | Cold outreach, inbound discovery | ✅ Active |
| 02 | Customer Journey Mirror | [Video 2](https://www.youtube.com/watch?v=FCrJoBjya2c) | Post-demo close call | ✅ Active |
| 03 | Warm Referral | TBD | Referral calls | ⏳ Pending |
| 04 | Price-First Qualification | TBD | Price shoppers | ⏳ Pending |
| 05 | De-escalation | TBD | Complaints | ⏳ Pending |
| 06 | Demo Follow-up | TBD | No-response after demo | ⏳ Pending |
| 07 | Win-Back | TBD | Churned clients | ⏳ Pending |
| 08 | Event Follow-up | TBD | Conference/event leads | ⏳ Pending |
| 09 | Voicemail Drop | TBD | First voicemail | ⏳ Pending |
| 10 | Breakup Voicemail | TBD | Final attempt | ⏳ Pending |

## Platform & Operations References

| ID | Name | Source | Best For | Status |
|----|------|--------|----------|--------|
| P1 | GHL A2P Registration | [Video 3](https://www.youtube.com/watch?v=wGhJHiRlI_8) | Client onboarding, texting setup | ✅ Active |

## Pricing & Positioning References

| ID | Name | Source | Best For | Status |
|----|------|--------|----------|--------|
| PP1 | Pricing & Positioning Data | Consolidated from all videos | All sales calls | ✅ Active |

---

## Video Library

| # | URL | Type | What We Learned |
|---|-----|------|----------------|
| 1 | https://www.youtube.com/watch?v=CqE7lEaIckE | Technique | Research-first cold calling, survey framework, pain math |
| 2 | https://www.youtube.com/watch?v=FCrJoBjya2c | Technique | Customer Journey Mirror post-demo close |
| 3 | https://www.youtube.com/watch?v=wGhJHiRlI_8 | Platform | A2P registration, texting stats, $1K/mo pricing benchmark |
