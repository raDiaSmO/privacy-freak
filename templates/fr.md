# Lettres — français

**Deux types de champs, jamais confondus :**

- **`{{DOUBLES ACCOLADES}}` — c'est l'assistant qui les remplit**, à partir du tableau des
  juridictions dans `SKILL.md`, avant d'afficher le brouillon. Aucune ne doit subsister dans la
  sortie.
- **`[CROCHETS SIMPLES]` — c'est la personne qui les remplit**, dans son logiciel de courriel. Ils
  doivent rester intacts. N'y substituez jamais de vraies données personnelles.

Gardez la lettre aussi courte qu'ici. Une action, une base légale, une date, une seule chose
demandée en retour. N'étoffez pas.

---

## A — Demande de suppression, avec un compte

**Objet :** Demande de suppression de renseignements personnels — {{LAW}} — [ACCOUNT EMAIL]

```
À : [CONTACT VIE PRIVÉE, TEL QUE PUBLIÉ DANS LA POLITIQUE]

Madame, Monsieur,

Veuillez supprimer tous les renseignements personnels que vous détenez à mon
sujet.

Compte : [ACCOUNT EMAIL]
[ACCOUNT ID — si connu]

Je réside à [CITY, PROVINCE/STATE] et je formule cette demande en vertu de
{{LAW}}, {{PROVISION}}. Votre délai pour répondre est de {{DEADLINE}}.

{{JURISDICTION SENTENCE}}

Veuillez me confirmer par écrit lorsque la suppression sera faite. Si vous
devez conserver quelque chose, indiquez-moi quoi et en vertu de quelle
obligation légale.

[NAME]
[DATE]
```

---

## B — Demande de suppression, sans compte

Pour les courtiers en données, les sites de recherche de personnes et les listes marketing.

**Objet :** Demande de suppression de renseignements personnels — {{LAW}} — sans compte

```
À : [CONTACT VIE PRIVÉE, TEL QUE PUBLIÉ DANS LA POLITIQUE]

Madame, Monsieur,

Veuillez supprimer tous les renseignements personnels que vous détenez à mon
sujet. Je n'ai aucun compte chez vous ; mes renseignements ont été recueillis
auprès d'autres sources.

Pour retrouver mes dossiers :
[NAME]
[CITY, PROVINCE/STATE]
[ACCOUNT EMAIL]

Je réside à [CITY, PROVINCE/STATE] et je formule cette demande en vertu de
{{LAW}}, {{PROVISION}}. Votre délai pour répondre est de {{DEADLINE}}.

{{JURISDICTION SENTENCE}}

Veuillez me confirmer par écrit lorsque la suppression sera faite, et ne pas
me réintégrer à partir de vos sources en amont.

[NAME]
[DATE]
```

Sans la dernière phrase, un courtier peut supprimer la fiche et la réintégrer au prochain
rafraîchissement.

---

## C — Relance, délai dépassé

Répondez dans le fil d'origine : c'est votre preuve de la date d'envoi.

**Objet :** Deuxième avis — demande de suppression du [DATE OF ORIGINAL REQUEST] — [ACCOUNT EMAIL]

```
À : [CONTACT VIE PRIVÉE, TEL QUE PUBLIÉ DANS LA POLITIQUE]

Madame, Monsieur,

Le [DATE OF ORIGINAL REQUEST], je vous ai demandé de supprimer tous les
renseignements personnels que vous détenez à mon sujet. Demande initiale
ci-dessous.

Compte : [ACCOUNT EMAIL]

Votre délai en vertu de {{LAW}} était le [DEADLINE DATE]. Je n'ai reçu aucune
réponse satisfaisante.

Veuillez me confirmer la suppression par écrit dans les 10 jours. À défaut, je
déposerai une plainte auprès de {{REGULATOR}} le [FINAL DEADLINE DATE] en
joignant la présente correspondance.

[NAME]
[DATE]

--- Demande initiale, envoyée le [DATE OF ORIGINAL REQUEST] ---
[COLLER ICI LE COURRIEL D'ORIGINE]
```

---

## Phrase de juridiction — une seule, ou aucune

La plupart des lettres n'ont besoin de rien ici. N'ajoutez une phrase que là où elle travaille
vraiment.

**Québec** — seulement si les renseignements sont publiés ou indexés quelque part :

```
Veuillez également cesser de diffuser ces renseignements et désindexer tout
hyperlien associé à mon nom, en vertu de l'article 28.1.
```

**Canada (LPRPDE)** — nécessaire, car la LPRPDE n'a pas de droit autonome à l'effacement et le
retrait du consentement sert de base :

```
Je retire mon consentement à la collecte, à l'utilisation et à la
communication de mes renseignements personnels, qui ne sont donc plus
nécessaires à aucune fin à laquelle j'ai consenti.
```

**UE / EEE / Royaume-Uni** — l'article 17 se suffit à lui-même ; n'ajoutez rien par défaut. Si la
personne reçoit de la prospection :

```
Je m'oppose également à tout traitement de mes données à des fins de
prospection directe, au titre de l'article 21, paragraphe 2.
```

**Californie** — nécessaire, sinon ils ne suppriment que leur propre copie :

```
Veuillez également ordonner à vos prestataires et sous-traitants de les
supprimer, en vertu du § 1798.105(c)(1), et traiter la présente comme un refus
de la vente et du partage.
```

Pour un **courtier en données** californien, le Delete Act de l'État (SB 362) a créé un mécanisme de
suppression centralisé (DROP) qui atteint tous les courtiers enregistrés en une seule demande. Son
calendrier a été modifié à plusieurs reprises : **vérifiez l'état actuel sur le site de la CPPA
avant de le mentionner**, et traitez-le comme un complément à la lettre B, jamais un remplacement.

---

## Ajouts optionnels — seulement si la personne les demande

Chacun transforme une demande de suppression en demande d'accès par surcroît. C'est plus de travail
pour le destinataire, et un motif légitime de prendre toute la prolongation. Proposez-les, dites ce
qu'ils coûtent, et laissez-les de côté par défaut.

- *Que déteniez-vous, et d'où ça vient ?* — RGPD art. 14(2)(f), CCPA § 1798.115.
- *À qui l'avez-vous communiqué ?* — le RGPD art. 19 les oblige à notifier l'effacement aux
  destinataires.
- *Confirmez la suppression des sauvegardes, pas seulement des systèmes actifs.*
- *Transmettez à vos sous-traitants et sociétés affiliées, et nommez-les.*

Si ce que la personne veut vraiment, c'est savoir ce qu'une entreprise détient, c'est une demande
d'accès distincte, envoyée après confirmation de la suppression.
