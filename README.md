# Reverse-Phone

**Le téléphone arabe… à l'envers.** Un party game vocal à jouer entre potes, en ligne ou sur un seul appareil.

**Jouer : https://tonpseudo.github.io/Reverse-Phone/**

## Le principe

Un mot circule de joueur en joueur, toujours joué **à l'envers**. À ton tour :

1. Tu écoutes le son reçu (du charabia, c'est normal)
2. Tu l'imites à voix haute
3. Tu écoutes ta tentative remise à l'endroit — ton seul indice
4. Tu dis clairement ce que tu as cru comprendre
5. Tu ajoutes ton propre mot, qui repart à l'envers chez le suivant

À la fin, révélation : la **vraie phrase** (ce qui a été dit) face à la **phrase perçue** (ce que tout le monde a compris). Spoiler : c'est jamais pareil.

## Modes de jeu

- **En ligne** — un joueur crée un salon, partage le code à 4 lettres, chacun joue depuis chez lui
- **En local** — un seul appareil qu'on se passe de main en main

Réglages : nombre de mots (2-20) et temps par tour (15-120 s, chrono avec compte à rebours).

## Côté technique

- Un seul fichier HTML, zéro installation, zéro backend
- Multijoueur en **pair-à-pair (WebRTC via PeerJS)** : la partie est hébergée dans l'onglet du créateur du salon, les sons circulent directement entre navigateurs
- Micro requis (autorisation demandée une seule fois) — fonctionne sur mobile via ce lien HTTPS

## Limites connues

- Si l'hôte ferme son onglet, la partie s'arrête
- Sur certains réseaux très restrictifs (wifi d'entreprise…), la connexion directe peut échouer