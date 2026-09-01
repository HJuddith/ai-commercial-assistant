# 🤖 AI Commercial Assistant

> Prototype d'assistant commercial basé sur l'IA agentique et l'automatisation.

## 📌 Présentation

**AI Commercial Assistant** transforme les données prospects en recommandations commerciales grâce à un **AI Agent**, des workflows automatisés et une interface web.

### Fonctionnalités

- Qualification et scoring des prospects
- Priorisation
- Identification des informations manquantes
- Recommandation de prochaine action
- Génération de messages personnalisés
- Mise à jour automatique des données
- Validation humaine avant toute action externe

## 🧠 IA agentique

L'agent analyse un prospect, utilise les outils disponibles et produit une recommandation structurée.

```text
Prospect
   ↓
Airtable
   ↓
n8n
   ↓
AI Agent
   ↓
Analyse + Score + Priorité
   ↓
Action recommandée
   ↓
Message personnalisé
   ↓
Validation humaine
```

## Architecture

```
Frontend
   ↓
Webhook
   ↓
n8n
   ↓
AI Agent
   ├── LLM
   ├── Airtable
   └── Knowledge Base
   ↓
Airtable
   ↓
Validation humaine

```

### Architecture finale du projet

```
ai-commercial-assistant/
│
├── frontend/                 # Application React
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── types/
│   │   └── App.tsx
│   ├── package.json
│   └── ...
│
├── n8n/
│   ├── workflows/
│   │   └── ai-commercial-agent.json
│   └── README.md
│
├── airtable/
│   ├── schema.md
│   └── sample-data.csv
│
├── prompts/
│   ├── system-prompt.md
│   └── qualification-rules.md
│
├── knowledge/
│   ├── services.md
│   └── faq.md
│
├── docs/
│   ├── architecture.md
│   └── screenshots/
│
├── .gitignore
├── README.md
└── LICENSE
```

## 🛠️ Stack technique

| Technologie  | Rôle                           |
| ------------ | ------------------------------ |
| React        | Interface utilisateur          |
| TypeScript   | Frontend                       |
| Tailwind CSS | UI                             |
| n8n          | Automatisation & orchestration |
| Airtable     | Données prospects              |
| LLM          | Génération & analyse           |
| AI Agent     | Qualification & décision       |
| Git / GitHub | Versionnement                  |

## 🎓 Objectif du projet

- Centraliser les informations prospects
- Automatiser la qualification des prospects
- Évaluer leur niveau de pertinence
- Attribuer un score et une priorité
- Identifier les informations manquantes
- Recommander la prochaine meilleure action
- Générer un message commercial personnalisé
- Mettre à jour automatiquement les données
- Conserver une validation humaine avant toute communication externe

---

Ce projet constitue un exercice pratique de Product Building, Low-Code/No-Code, automatisation et IA agentique.

Il permet d'explorer la conception d'un produit de bout en bout :

```
Problème métier
      ↓
Conception produit
      ↓
Modèle de données
      ↓
Automatisation
      ↓
AI Agent
      ↓
Interface utilisateur
      ↓
Validation humaine
      ↓
Tests
      ↓
Documentation
```

🔐 Confidentialité

Projet indépendant et générique utilisant exclusivement des données fictives.

Aucune donnée, information interne ou donnée confidentielle d'une entreprise réelle n'est utilisée.
