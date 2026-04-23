# CLAUDE.md Template — L'OS de ton bras droit IA

> Le fichier que Claude Code lit AU-DESSUS de tout. Celui qui fait la différence entre un chatbot et un associé.

## Ce que c'est

**CLAUDE.md** est un fichier que tu places à la racine de ton dossier projet (ou dans `~/.claude/CLAUDE.md` pour qu'il soit lu dans TOUTES tes sessions Claude Code).

Claude Code le lit automatiquement à chaque ouverture. Il devient le "system prompt permanent" de ton IA : ton identité, tes règles, ton métier, ton ton, ce que tu refuses, ce que tu veux.

Bien écrit, tu ne redis plus jamais la même chose. Tu ouvres un terminal, tu tapes 3 mots, ton Claude sait quoi faire.

---

## Comment utiliser ce template

### Option A — Claude Code (CLI)

```bash
# 1. Télécharger le template
curl -O https://raw.githubusercontent.com/antonioilinca/claude-md-template/main/CLAUDE.md

# 2. Placer au bon endroit
# Pour TOUTES les sessions (recommandé) :
mv CLAUDE.md ~/.claude/CLAUDE.md

# Ou pour un projet spécifique uniquement :
mv CLAUDE.md /chemin/vers/ton/projet/CLAUDE.md
```

### Option B — Claude Desktop / claude.ai

Copie le contenu de `CLAUDE.md` dans :
- **Claude Desktop** : Settings → Custom Instructions
- **claude.ai** (web) : icône profil → Settings → Personalization → Custom Instructions

---

## Ce que tu dois remplir

Le template contient des zones `{MAJUSCULES}` à remplacer par tes infos.

### Section "Identité"

| Placeholder | Ce que tu dois mettre |
|---|---|
| `{TON_PRENOM}` | Ton prénom. C'est comme ça que l'IA te nommera en interne. |
| `{TON_METIER}` | Ton rôle en 2-4 mots. "Freelance dev web", "Consultant RH", "Fondateur SaaS", "Étudiant en école d'ingé". |
| `{TON_AGE}` | Ton âge (optionnel — utile si tu veux que l'IA adapte son ton). |
| `{TA_VILLE}` | Ta ville (utile pour les infos locales : fiscalité, marché, réseaux). |
| `{TON_POSTE_OU_BUSINESS}` | Contexte pro en 1 ligne. "Salarié chez X", "Fondateur solo sans employés", "Consultant 3 jours/semaine". |

### Section "North Star"

| Placeholder | Ce que tu dois mettre |
|---|---|
| `{TA_METRIQUE_UNIQUE}` | **La** métrique qui compte. Pas 3, pas 5. UNE. Exemples : "1ère vente de mon SaaS", "10 clients facturés", "10k€ MRR", "Mission freelance signée", "Code livré en prod". |
| `{VALEUR_ACTUELLE}` | Où tu en es aujourd'hui. "0 vente", "2 clients", "4 200€ MRR", "0 feature shippée". |
| `{DATE}` | Date de la mise à jour. Format YYYY-MM-DD. |
| `{LA_METRIQUE}` | Reformulation ultra-courte de ta North Star pour la jauge de décision. |

### Section "Ce que je fais"

| Placeholder | Ce que tu dois mettre |
|---|---|
| `{TA_CONTRAINTE_BUDGET}` | Ta règle d'argent. "Tout gratuit par défaut", "Max 50€/mois en outils", "Pas de dépense sans valider". |
| `{TON_OFFRE_OU_LIVRABLE}` | Ce que tu vends ou ce que tu livres. "Formation X à Y€", "Mission freelance dev React", "Feature Y pour équipe interne". |
| `{TA_PRIORITE_AUJOURDHUI}` | Ce qui prime cette semaine. "La 1ère vente, pas la feature parfaite", "Livrer la v1 avant la démo", "Trouver 3 clients d'ici vendredi". |
| `{DECRIS_TON_CONTEXTE_EN_3_LIGNES}` | Qui tu es, ce que tu construis, avec qui tu bosses. 3 lignes max. |
| `{TON_DOMAINE}` | Ton domaine principal. "marketing", "dev", "data", "OSINT", "RH", etc. Sert à nommer les dossiers `references/{TON_DOMAINE}-procedures.md`. |

---

## Pourquoi ça marche

### 1. **Une seule métrique** (North Star)

Tu empêches l'IA de construire des features qui n'avancent pas ton but. Chaque action passe la jauge "ça sert la North Star ?". Si non → alerte. Ça coupe 80% du bruit.

### 2. **10 règles absolues**

L'IA a un cadre de décision permanent. Tu n'as plus besoin de répéter à chaque message : "sois direct", "pas de disclaimer", "français avec accents", "pas de corporate". Tu l'écris une fois, c'est appliqué toujours.

### 3. **Mode discret**

L'IA connaît TOUT sur toi (profil, sujets sensibles, zones rouges) mais ne récite jamais. Elle utilise l'info comme un outil, pas comme un script. Par exemple, elle sait que tu détestes qu'on te parle de ton ancien échec business, donc elle ne le mentionne pas — sauf si tu l'abordes toi.

### 4. **Activation auto des skills**

Tu définis des déclencheurs en langage naturel :
- "y'a un bug" → l'IA lance ton workflow `/investigate`
- "déploie" → `/ship` + check canary
- "écris un post" → `/linkedin-post` avec anti-doublon auto

Plus de syntaxe slash à mémoriser.

### 5. **The Most Lazy Guy Rule**

L'IA fait tout elle-même. Zéro "peux-tu lancer cette commande stp ?". Elle lance, rapporte. Si une auth interactive est nécessaire, elle affiche la commande pour que tu la lances toi-même.

---

## Conseils pour un bon CLAUDE.md

### À faire

- **Être spécifique, pas générique.** "Réponds en français avec accents" > "Réponds proprement".
- **Lister les règles en dur.** L'IA ne devine pas — elle exécute ce qui est écrit.
- **Mettre une North Star unique.** Si tu mets 3 objectifs, l'IA va diluer.
- **Anticiper les sujets sensibles.** Liste ce que l'IA ne doit jamais évoquer spontanément.
- **Mettre des exemples concrets** de ton ton et de ton style.
- **Relire toutes les semaines.** Un CLAUDE.md obsolète = IA qui te ralentit.

### À éviter

- **Le corporate vague.** "Être professionnel et bienveillant" ne sert à rien.
- **Les règles contradictoires.** "Sois court mais complet et détaillé" → l'IA choisira au hasard.
- **Les secrets en clair.** JAMAIS de clés API, tokens, mots de passe dans le CLAUDE.md. Il peut être lu par tout outil qui accède au dossier.
- **Le "tu peux".** Utilise l'impératif. "Rapporte en 2 phrases max" > "Tu peux rapporter brièvement".

---

## Structure recommandée autour du CLAUDE.md

```
~/.claude/
├── CLAUDE.md                      ← le fichier principal (ce template)
├── memory/                        ← mémoire persistante entre sessions
│   ├── MEMORY.md                  ← index des mémoires
│   ├── feedback-regles.md         ← tes corrections IA à respecter
│   └── context-business.md        ← ton contexte pro à jour
└── references/                    ← procédures, erreurs, checklists
    ├── erreurs.md                 ← erreurs à ne JAMAIS refaire
    └── procedures.md              ← workflows détaillés
```

---

## Comment tester que ton CLAUDE.md marche

1. Écris-le avec tous les placeholders remplis.
2. Place-le dans `~/.claude/CLAUDE.md`.
3. Ouvre un nouveau terminal, lance `claude` (ou la commande que tu utilises).
4. Pose une question **courte** sur ton métier sans donner de contexte. Exemple : "fais-moi un post LinkedIn".
5. Si l'IA respecte ton ton, ta North Star et tes règles sans que tu les répètes → ça marche.
6. Si elle répond de manière générique → ton CLAUDE.md est trop vague. Re-spécifie.

---

## Licence

MIT — fais ce que tu veux. Si ça t'aide, un lien vers ce repo en retour est apprécié.

## Contribuer

Une amélioration ? Une section qui devrait être là ? Ouvre une issue ou une PR.
