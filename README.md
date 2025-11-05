# Bataille Navale — Centrale Méditerranée

**Version du projet :** `v2.0.0`
**Version Python recommandée :** `3.13.7`

## Description

Jeu de **Bataille Navale** développé en **Python** pour **un joueur**.
Le jeu se joue dans le **terminal** et propose deux modes : `test` (affiche les bateaux) et `default` (bateaux masqués).

## Objectif

Coder un jeu de bataille navale avec une interface terminal pour un seul joueur. La partie se termine lorsque tous les bateaux sont détruits. Un score final est calculé en fonction du nombre de tirs effectués.

---

## Spécifications — `v2.0.0`

### Grille de jeu

* Taille : **8 lignes × 10 colonnes**

### Bateaux (placés aléatoirement)

| Symbole | Nom du bateau |
| ------- | ------------- |
| 🚢      | Porte-avion   |
| ⛴       | Croiseur      |
| 🚣      | Torpilleur    |
| 🐟      | Sous-marin    |

### Modes de jeu

* `test` : les bateaux sont visibles (utile pour le débogage ou les démonstrations).
* `default` : les bateaux sont masqués (mode de jeu normal).

### Convention de coordonnées

Les coordonnées saisies dans le terminal commencent à **1** (et non 0).

Exemples valides :

* `(1, 1)` — coin haut-gauche
* `(1, 10)` — première ligne, dernière colonne
* `(8, 1)` — dernière ligne, première colonne
* `(8, 10)` — coin bas-droit

Exemples invalides :

* `(0, 0)`, `(0, 1)`, `(1, 0)` — **ne pas utiliser**

---

## Règles de la partie

* Les bateaux sont placés **aléatoirement** au début de la partie.
* Le joueur effectue des tirs en saisissant des coordonnées dans le terminal.
* La partie se termine une fois **tous** les bateaux détruits.
* Un **score final** est attribué en fonction du nombre de tirs effectués (moins de tirs = meilleur score).

---

## Installation et exécution (Windows)

Ouvrir un terminal dans le dossier du projet et exécuter :

```bash
# créer un environnement virtuel
python -m venv venv/

# activer l'environnement (Windows)
venv\Scripts\activate

# installer les dépendances
venv\Scripts\python -m pip install -r requirements.txt

# lancer le jeu
python main.py
```

**Remarque** : sous macOS / Linux, activez l'environnement avec :

```bash
source venv/bin/activate
```

---

## Récupération du projet depuis GitHub

Cloner le dépôt (branche `main`) :

```bash
git clone -b main https://github.com/Edouard13013/BatailleNavale.git
```

Lister les tags / versions disponibles :

```bash
git tag
```

Utiliser une version spécifique (ex. `v2.0.0`) :

```bash
git checkout v2.0.0
```

---

## Versions

* `1.0.0` — version test initiale
* `v2.0.0` — version de jeu stable (spécifications ci-dessus)

---

## Idées & évolutions futures

* Interface graphique (hors terminal)
* Génération de grilles non rectangulaires et plus de types de bateaux
* Modes de difficulté : `facile` (radar), `difficile` (bateaux en mouvement entre les tirs)
* Types de tirs supplémentaires (salve, sonar, etc.)

---

## Licence & contribution

Ajoutez une licence et un fichier `CONTRIBUTING.md` si vous souhaitez accepter les contributions.
Pour toute question ou suggestion, créez une *issue* sur le dépôt GitHub.

---

Bonne partie ⚓️
