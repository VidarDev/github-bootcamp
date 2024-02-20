<!-- slides.md -->

# The Ultimate Git Cheat Sheet

---

## Introduction
**Git & Oh My Zsh**: Deux outils puissants pour les développeurs.  
Découvrez comment les utiliser efficacement.  
Pour plus de détails, visitez [le cheat sheet de David Leuliette](https://davidl.fr/blog/git-cheatsheet).

---

## Configuration Initiale
- **Oh My Zsh**: Un framework pour gérer votre configuration Zsh.
- **Installation**: Suivez les [étapes pour configurer git et oh-my-zsh`](https://davidl.fr/blog/git-cheatsheet#section-1).

---

## Commandes de Base
- **Statut**: pour un aperçu rapide.

```
gss
```

- **Ajout de Fichiers**: pour ajouter tous les fichiers.

```
gaa
```

---

## Visualisation des Commits
- **Historique**: pour une vue graphique.

```
glgg
```

- **Détails des Commits**: montre plus d'informations.

```
glol
```

---

## Gestion des Branches
- **Création de Branches**: Apprenez à créer et à changer de branches.
- **Fusion**: Techniques de fusion pour maintenir l'intégrité du code.

---

## Travail Collaboratif
- **Pull Requests**: La clé pour une collaboration efficace.
- **Résolution de Conflits**: Techniques pour gérer les conflits.

---

## Création d'alias

Remplacez **"Votre nom complet"** par le nom associé à vos commits dans Git.
Cette commande crée un alias nommé today qui exécute la commande log de Git avec des paramètres spécifiques pour filtrer les commits de la journée actuelle.

```
git config --global alias.today "log --since=midnight --author='Votre nom complet' --oneline"
```

---

- Sélectionne les commits faits depuis minuit aujourd'hui.
```
--since=midnight
```

- Filtre les commits pour n'afficher que ceux faits par l'auteur spécifié.

```
--author='Votre nom complet
```

- Affiche chaque commit sur une seule ligne pour une meilleure lisibilité.

```
--oneline
```

---

## Gestion des Branches avec Git

---

## Créer une Nouvelle Branche
- **Commande**: `git branch feature/branching`
- **Description**: Cette commande crée une nouvelle branche nommée `feature/branching`.
- **Contexte**: Idéal pour développer de nouvelles fonctionnalités en parallèle.

---

## Travailler sur une Branche
- **Commande**: `git checkout feature/branching`
- **Focus**: Faire des changements spécifiques à une fonctionnalité sur cette branche.
- **Avantage**: Sépare le développement de nouvelles fonctionnalités du travail principal.

---

# Gestion de Branches avec Git

---

## Créer une nouvelle branch : `feature/swag`
- **Commande**: `git branch feature/swag`
- **Description**: Création d'une branche pour le développement de la fonctionnalité 'swag'.

---

## Basculer vers la branch principale
- **Commande**: `gcm` (alias pour `git checkout main`)
- **Description**: Revenir à la branche principale avant la fusion.

---

## Fusionner la branch `feature/swag`
- **Commande**: `git merge feature/swag`
- **Description**: Intégrer les changements de la branche `feature/swag` dans la branche principale.

---

# Création de Slides en Markdown

---

## Slide: Texte

Ajoutez du texte de démonstration ici.

```markdown
texte de démonstration ici.
```

---

## Slide: Listes

Créer des exemples de listes à puces ou numérotées.

```markdown
- Item 1
- Item 2
```

---

## Slide: Images

Insérer une image de démonstration.

```markdown
![My Image](https://i.imgur.com/1.png)
```

---

## Slide: En-têtes & Citations
Exemples d'utilisation d'en-têtes et de citations.

```markdown
# En-tête de premier niveau
## En-tête de deuxième niveau
### En-tête de troisième niveau
```

```markdown
`Text`
```

---

## Slide: Code
Afficher un exemple de bloc de code.

```markdown
```
code
```
```

---

## Slide: Extras
Ajouter des informations supplémentaires ou des astuces.

```markdown
> Ajouter des informations supplémentaires
```

---

## Transférer les modifications à distance

Envoyez vos commits vers le référentiel distant. Utiliser:
```console
git push origin main
```

---

## Extraire les modifications depuis le remote

- Pour mettre à jour votre repository local avec le dernier commit du remote repository, utilisez :

```console
git push origin main
```

- Remplacez `branch_name` par le nom de la branche à partir de laquelle vous souhaitez extraire. Si vous travaillez avec la branche principale, il s'agit souvent de `main` ou `master`.

---

## Conclusion

La **gestion des branches** est essentielle pour une collaboration efficace et une maintenance claire du code.

**Git** et **Oh My Zsh** sont des outils essentiels pour améliorer votre flux de travail.  
Retrouvez plus de conseils et de commandes [sur le site de David Leuliette](https://davidl.fr/blog/git-cheatsheet).