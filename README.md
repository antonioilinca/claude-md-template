# CLAUDE.md Template — L'OS de ton bras droit IA

> Le fichier que Claude Code lit AU-DESSUS de tout. Celui qui fait la différence entre un chatbot et un associé.

## Ce que c'est

**CLAUDE.md** est un fichier que tu places à la racine de ton dossier projet (ou dans `~/.claude/CLAUDE.md` pour qu'il soit lu dans TOUTES tes sessions).

Claude Code le lit automatiquement à chaque ouverture. Il devient le "system prompt permanent" de ton IA : ton identité, tes règles, ton métier, ton ton, ce que tu refuses, ce que tu veux.

Bien écrit, tu ne redis plus jamais la même chose. Tu ouvres un terminal, tu tapes 3 mots, ton Claude sait quoi faire.

---

## Comment utiliser ce template

### Option A — Claude Code (CLI)

```bash
# 1. Télécharger
curl -O https://raw.githubusercontent.com/antonioilinca/claude-md-template/main/CLAUDE.md

# 2. Placer au bon endroit
# Pour TOUTES les sessions (recommandé) :
mv CLAUDE.md ~/.claude/CLAUDE.md

# Ou pour un projet spécifique :
mv CLAUDE.md /chemin/vers/ton/projet/CLAUDE.md
```

### Option B — Claude Desktop / claude.ai

Copie le contenu de `CLAUDE.md` dans :
- **Claude Desktop** : Settings → Custom Instructions
- **claude.ai** (web) : icône profil → Settings → Personalization → Custom Instructions

---

## Remplir les placeholders

Le template contient des zones `{MAJUSCULES}` à remplacer par tes infos :

| Placeholder | Exemple |
|---|---|
| `{TON_PRENOM}` | Antonio |
| `{TON_METIER}` | Entrepreneur IA / Freelance dev / Consultant |
| `{TON_AGE}` | 21 |
| `{TA_VILLE}` | Nantes |
| `{TON_POSTE_OU_BUSINESS}` | Fondateur solo, SaaS en prod |
| `{TA_METRIQUE_UNIQUE}` | 1ère vente formation / 10 clients / 10k MRR |
| `{VALEUR_ACTUELLE}` | 0 vente / 3 clients / 2 500€ MRR |
| `{DATE}` | 2026-04-23 |
| `{LA_METRIQUE}` | ta North Star (reformulée courte) |
| `{TA_CONTRAINTE_BUDGET}` | "Tout gratuit" ou "Maxi 50€/mois en outils" |
| `{TON_OFFRE_OU_LIVRABLE}` | Formation Claude 47€ / Mission freelance |
| `{TA_PRIORITE_AUJOURDHUI}` | La 1ère vente, pas la feature parfaite |
| `{DECRIS_TON_CONTEXTE_EN_3_LIGNES}` | Qui tu es, ce que tu construis, avec qui |
| `{TON_DOMAINE}` | marketing / dev / OSINT / etc. |

---

## Pourquoi ça marche

### 1. **Une seule métrique** (North Star)
Tu empêches l'IA de construire des features qui n'avancent pas ton but. Chaque action passe la jauge "ça sert la North Star ?".

### 2. **10 règles absolues**
L'IA a un cadre de décision. Pas besoin de répéter "sois direct", "français avec accents", "pas de disclaimer" à chaque message.

### 3. **Mode discret**
L'IA connaît TOUT sur toi mais ne récite jamais. Elle utilise l'info comme un outil, pas comme un script.

### 4. **Activation auto des skills**
Tu dis "y'a un bug" → l'IA lance `/investigate`. Tu dis "déploie" → `/ship`. Pas de syntaxe à mémoriser.

### 5. **The Most Lazy Guy Rule**
L'IA fait tout elle-même. Zéro "peux-tu lancer cette commande stp ?". Elle lance, rapporte.

---

## Exemples de CLAUDE.md réels (inspirations)

- **Le mien** (Antonio, 21 ans, Nantes, entrepreneur IA solo) : 9 agents 24/7, formation Claude 47€ — [cortex-flame-one.vercel.app/maitrise-claude](https://cortex-flame-one.vercel.app/maitrise-claude)

---

## Tu veux aller plus loin

La **formation Maîtrise Claude** (47€) couvre :
- Écrire un CLAUDE.md qui booste la qualité ×10
- Les 51 skills custom que j'utilise quotidiennement
- Brancher Claude sur tes outils (MCP, API, agents autonomes)
- Ship ton 1er SaaS en 7 jours sans coder

→ [cortex-flame-one.vercel.app/maitrise-claude](https://cortex-flame-one.vercel.app/maitrise-claude) (47€ au lieu de 497€, accès à vie, garantie 14j)

---

## Licence

MIT — fais ce que tu veux, mentionne la source si ça t'aide.

## Contribuer

Une amélioration ? Une section qui devrait être là ? Ouvre une issue ou une PR.
