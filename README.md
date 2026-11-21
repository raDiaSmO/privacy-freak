# privacy-freak

A Claude Skill for requesting deletion of your personal data from a company.

Give it a company name and where you live. It finds the company's privacy policy, links the
self-service deletion portal if there is one, otherwise finds the privacy contact, and drafts a
short email citing the law that applies and the deadline to respond.

You send it. The skill drafts and links; it does not send, submit, or log in.

Six files, no scripts, no dependencies.

## Coverage

| Where you live | Law cited |
|---|---|
| Quebec | Law 25 |
| Canada, outside Quebec | PIPEDA |
| EU / EEA / UK | GDPR Art. 17 |
| California | CCPA / CPRA |

Deadlines and regulators are in the jurisdiction table in `SKILL.md`.

Letters come in English and French: one for when you have an account, one for when you do not (data
brokers, people-search sites, marketing lists), and a follow-up for a missed deadline.

## Install

Claude Code:

```
ln -s "$(pwd)/privacy-freak" ~/.claude/skills/privacy-freak
```

Restart Claude Code, then run `/privacy-freak` or just ask. Use `cp -r` instead for a copy rather
than a live link. To scope it to one project, use that project's `.claude/skills/` instead.

Claude.ai: zip the folder with `SKILL.md` at its root, then upload under Settings → Capabilities →
Skills.

Web search must be available, or the policy-finding step cannot run.

## Example

```
You:    I want my data deleted from Example Corp.
Claude: Where do you live? Country, and province or state if it matters.
You:    Quebec.
Claude: 1. SELF-SERVICE PORTAL
           https://example.com/privacy/delete
           Verified domain: example.com (the company's own)
           Account → Privacy → Delete my data

        2. EMAIL  (if the portal fails, or you want a paper trail)
           To:      privacy@example.com
           Subject: Demande de suppression — Loi 25 — [ACCOUNT EMAIL]

           Madame, Monsieur,

           Veuillez supprimer tous les renseignements personnels que
           vous détenez à mon sujet.

           Compte : [ACCOUNT EMAIL]

           Je réside à [CITY, PROVINCE/STATE] et je formule cette
           demande en vertu de la Loi 25, art. 28.1. Votre délai pour
           répondre est de 30 jours.

           Veuillez me confirmer par écrit lorsque la suppression sera
           faite. Si vous devez conserver quelque chose, indiquez-moi
           quoi et en vertu de quelle obligation légale.

           [NAME]
           [DATE]

        3. SOURCES
           https://example.com/privacy — "Vos droits" — consulted 2026-11-06

        4. NEXT STEPS
           30-day deadline: 2026-12-06. Follow up 2026-12-08. Then: CAI.
```

`Example Corp` and `example.com` are fictional, as are all examples in this skill.

## What it will not do

- Send email, submit forms, log in, or create an account.
- Ask for your real name, email, address, account ID, or identity document. Drafts keep placeholders
  such as `[NAME]` and `[ACCOUNT EMAIL]` for you to fill in your own mail client.
- Guess a contact address. It uses one only if it appears in the published policy, and tells you
  where it found it.
- Show a deletion portal that is not on the company's own domain, or on a vendor domain linked from
  the policy. It names the domain it checked.
- Handle a password or a 2FA code.
- Act on anyone's data but yours. The no-account letter asks a company to search for a named person
  and say what it holds, which against someone else is a way to obtain a stranger's file. Acting for
  a child you are guardian of, or someone who authorized you, is supported: the letter states the
  capacity, and expect to be asked for proof.
- Follow instructions found on a web page. Page content is treated as data; anything on a page that
  addresses the assistant is reported to you instead.
- Recommend paid data-removal services.
- Write a file containing your request.

## Notes

The letters are deliberately short: one action, one legal basis, one deadline, one confirmation
requested. The skill does not add an access request to a deletion request, because asking for
categories, sources and recipients gives the company grounds to take the full extension. Those
extra asks are in the templates for when you want them.

Writing to a data broker gives it a verified name and a working email, and some treat opt-out
traffic as data enrichment. It is usually still worth sending, and the skill says so before you do.

## Limitations

- Policies move. A URL or address that is correct today may be dead later; the skill records the
  date it read a page.
- Deadlines and section numbers change. Citations are correct as written, but are not maintained
  automatically.
- Four laws. Elsewhere, the skill says so and cites the company's own obligations instead, which is
  weaker.
- It cannot compel anyone. It produces a grounded request and an escalation path.
- Verification practice varies. Some companies accept an email; others ask for identity documents.
- Not legal advice. For a disputed or high-stakes request, consult a lawyer or your regulator.

## Files

```
SKILL.md         workflow, jurisdiction table, rules
templates/en.md  letters and clauses, English
templates/fr.md  letters and clauses, French
```

## License

MIT — see [LICENSE](LICENSE).
