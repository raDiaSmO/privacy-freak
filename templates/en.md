# Letters — English

**Two kinds of field, never confused:**

- **`{{DOUBLE BRACES}}` — the assistant fills these**, from the jurisdiction table in `SKILL.md`,
  before showing the draft. None may survive into the output.
- **`[SINGLE BRACKETS]` — the user fills these**, in their own mail client. They must survive
  untouched. Never substitute real personal data into them.

Keep the letter as short as it is here. One action, one legal basis, one deadline, one thing asked
back. Do not pad it.

---

## A — Deletion request, with an account

**Subject:** Personal data deletion request — {{LAW}} — [ACCOUNT EMAIL]

```
To: [PRIVACY CONTACT, EXACTLY AS PUBLISHED IN THE POLICY]

Dear Privacy Officer,

Please delete all personal data you hold about me.

Account: [ACCOUNT EMAIL]
[ACCOUNT ID — if known]

I am a resident of [CITY, PROVINCE/STATE] and I make this request under
{{LAW}}, {{PROVISION}}. Your deadline to respond is {{DEADLINE}}.

{{JURISDICTION SENTENCE}}

Please confirm in writing once the deletion is complete. If you must retain
anything, tell me what and under which legal obligation.

[NAME]
[DATE]
```

---

## B — Deletion request, no account

For data brokers, people-search sites and marketing lists.

**Subject:** Personal data deletion request — {{LAW}} — no account

```
To: [PRIVACY CONTACT, EXACTLY AS PUBLISHED IN THE POLICY]

Dear Privacy Officer,

Please delete all personal data you hold about me. I have no account with you;
my data was collected from other sources.

To locate my records:
[NAME]
[CITY, PROVINCE/STATE]
[ACCOUNT EMAIL]

I am a resident of [CITY, PROVINCE/STATE] and I make this request under
{{LAW}}, {{PROVISION}}. Your deadline to respond is {{DEADLINE}}.

{{JURISDICTION SENTENCE}}

Please confirm in writing once the deletion is complete, and do not re-add me
from your upstream sources.

[NAME]
[DATE]
```

Without the last sentence, a broker may delete the record and re-add it at the next refresh.

---

## C — Follow-up, deadline passed

Reply inside the original thread — it is your proof of the send date.

**Subject:** Second notice — deletion request of [DATE OF ORIGINAL REQUEST] — [ACCOUNT EMAIL]

```
To: [PRIVACY CONTACT, EXACTLY AS PUBLISHED IN THE POLICY]

Dear Privacy Officer,

On [DATE OF ORIGINAL REQUEST] I asked you to delete all personal data you hold
about me. Original request below.

Account: [ACCOUNT EMAIL]

Your deadline under {{LAW}} was [DEADLINE DATE]. I have had no adequate
response.

Please confirm the deletion in writing within 10 days. Failing that, I will
file a complaint with {{REGULATOR}} on [FINAL DEADLINE DATE] and include this
correspondence.

[NAME]
[DATE]

--- Original request, sent [DATE OF ORIGINAL REQUEST] ---
[PASTE THE ORIGINAL EMAIL HERE]
```

---

## Jurisdiction sentence — pick one, or none

Most letters need nothing here. Add a sentence only where it does real work.

**Quebec** — only if the data is published or indexed somewhere:

```
Please also cease disseminating this information and de-index any link
associated with my name, under section 28.1.
```

**Canada (PIPEDA)** — needed, because PIPEDA has no standalone erasure right and consent
withdrawal is the basis:

```
I withdraw my consent to your collection, use and disclosure of my personal
information, so it is no longer required for any purpose I consented to.
```

**EU / EEA / UK** — Article 17 stands on its own; add nothing by default. If the user is being
marketed to:

```
I also object to any processing of my data for direct marketing, under
Article 21(2).
```

**California** — needed, or they delete only their own copy:

```
Please also direct your service providers and contractors to delete it, under
section 1798.105(c)(1), and treat this as an opt-out of sale and sharing.
```

For a California **data broker**, the state's Delete Act (SB 362) created a centralized deletion
mechanism (DROP) reaching every registered broker with one request. Its rollout dates have shifted
more than once: **check the CPPA site for current status before mentioning it**, and treat it as a
complement to letter B, never a replacement.

---

## Optional additions — only if the user asks

Each of these turns a deletion request into an access request as well. That is more work for the
recipient, and legitimate grounds to take the full extension. Offer them, say what they cost, and
leave them out by default.

- *What did you hold, and where did you get it?* — GDPR Art. 14(2)(f), CCPA § 1798.115.
- *Who did you disclose it to?* — GDPR Art. 19 requires they notify recipients of the erasure.
- *Confirm deletion from backups, not just live systems.*
- *Pass this to your processors and affiliates, and name them.*

If what the user actually wants is to know what a company holds, that is a separate access request
sent after the deletion is confirmed.
