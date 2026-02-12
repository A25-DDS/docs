# Cours — Les tags Git

## 1. Qu’est-ce qu’un tag Git ?

Un **tag Git** est une **étiquette (label)** attachée à un commit spécifique.

Il sert à **marquer une version importante du projet**.

On peut voir un tag comme un **repère fixe dans l’historique du projet**.

---

## 2. Pourquoi utiliser des tags ?

Dans un projet réel, il peut y avoir :

- des centaines de commits
- des dizaines de fonctionnalités
- plusieurs versions publiées

Les tags permettent de :

- marquer une version stable
- retrouver rapidement une version précise
- publier une version officielle
- synchroniser avec Docker, CI/CD, etc.

---

## 3. Exemple concret

Historique des commits :

```
A --- B --- C --- D --- E --- F
                ↑     ↑
              v1.0  v1.1
```

Les tags :

- `v1.0` pointe vers le commit C
- `v1.1` pointe vers le commit E

Même si de nouveaux commits sont ajoutés, le tag reste fixe.

---

## 4. Convention de nommage : SemVer

On utilise généralement le **Semantic Versioning (SemVer)** :

```
vMAJEUR.MINEUR.CORRECTIF
```

Exemples :

```
v1.0.0
v1.1.0
v1.1.1
v2.0.0
```

Exemples fonctionnels :

```
v1.0.0 → Première version stable
v1.1.0 → Nouvelle fonctionnalité
v1.2.0 → Authentification JWT ajoutée
v1.2.1 → Correction bug auth
```

---

# 5. Les deux types de tags

Git possède deux types de tags :

- tag léger
- tag annoté

---

# 6. Tag léger (lightweight tag)

## Définition

Un tag léger est simplement un **pointeur vers un commit**.

Il ne contient aucune information supplémentaire.

On peut le comparer à une **branche fixe qui ne bouge jamais**.

---

## Création

Créer un tag sur le commit actuel :

```
git tag v1.0.0
```

Créer un tag sur un commit spécifique :

```
git tag v1.0. 7a38f12
```

---

## Stockage interne

Les tags légers sont stockés dans :

```
.git/refs/tags/
```

Chaque fichier contient le hash du commit.

Exemple :

```
.git/refs/tags/v1.0.0
```

Contenu :

```
7a38f1298ab45c...
```

---

# 7. Tag annoté (annotated tag)

## Définition

Un tag annoté est un **objet Git complet** contenant :

- le hash du commit
- le nom du créateur
- son email
- la date
- un message

C’est le type utilisé en production.

---

## Création

```
git tag -a v1.0.1 -m "Version 1.0.1 - auth fonctionnelle"
```

---

## Visualiser un tag annoté

```
git show v1.0.1
```

Exemple de sortie :

```
tag v1.0.1
Tagger: Jean Paul <jean@gmail.com>
Date: Mon Mar 23 14:34:08 2020

Version 1.0.1 - auth fonctionnelle

commit 02d954056df1bbbb29668c8d8247104f416e3bce
Author: Arthur <arthur@gmail.com>

Message du commit
```

---

# 8. Lister les tags

Afficher tous les tags :

```
git tag
```

Exemple :

```
v1.0.0
v1.0.1
v1.1.0
```

---

# 9. Se positionner sur un tag

On peut naviguer vers un tag :

```
git checkout v1.0.0
```

Git place alors le repository en **HEAD détachée**.

Cela permet de :

- voir le code à cette version
- tester une version spécifique

Mais pas de continuer le développement directement.

---

# 10. Supprimer un tag

Supprimer un tag local :

```
git tag -d v1.0.0
```

---

# 11. Modifier un tag

Modifier un tag local :

```
git tag -f v1.0.0 7a38f12
```

⚠️ Attention : ne jamais modifier un tag déjà partagé.

Pourquoi ?

Les autres développeurs auront une version différente.

Bonne pratique :

Créer un nouveau tag :

```
v1.0.1
```

et non modifier :

```
v1.0.0
```

---

# 12. Publier un tag

Par défaut, les tags ne sont pas envoyés sur le serveur.

Envoyer un tag spécifique :

```
git push origin v1.0.0
```

Envoyer tous les tags :

```
git push origin --tags
```

---

# 13. Voir les tags sur GitLab / GitHub

Sur GitLab :

Projet → Dépôt → Étiquettes

Sur GitHub :

Projet → Releases ou Tags

---

# 14. Workflow professionnel typique

Développement :

```
git commit
git commit
git commit
```

Publication d'une version :

```
git tag -a v1.0.0 -m "Version stable"
git push origin v1.0.0
```

---

# 15. Exemple concret complet

Créer un projet :

```
git init
```

Ajouter un fichier :

```
git add .
git commit -m "Version initiale"
```

Créer un tag :

```
git tag -a v1.0.0 -m "Première version stable"
```

Lister :

```
git tag
```

Voir :

```
git show v1.0.0
```

Publier :

```
git push origin v1.0.0
```

---

# 16. Résumé visuel

Historique :

```
A --- B --- C --- D --- E
      ↑     ↑     ↑
    v1.0  v1.1  v2.0
```

---

# 17. Bonnes pratiques professionnelles

Toujours utiliser :

```
tag annoté
```

Toujours utiliser :

```
semver
```

Ne jamais modifier un tag publié.

Toujours tagger les versions importantes :

- release
- production
- milestone

---

# 18. Lien avec Docker (industrie)

Git :

```
git tag v1.4.2
```

Docker :

```
docker build -t mon-app:1.4.2 .
```

---

# 19. Résumé simple à retenir

Un tag est :

→ une étiquette
→ une version
→ un pointeur fixe vers un commit

---

# 20. Commandes essentielles

Créer tag annoté :

```
git tag -a v1.0.0 -m "Version stable"
```

Lister :

```
git tag
```

Voir :

```
git show v1.0.0
```

Push :

```
git push origin v1.0.0
```
