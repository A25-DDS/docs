### **Kit Pédagogique : Story Mapping - Donnez du Sens à Votre Backlog !**

---

### **La Métaphore du Film (Pour Tout Comprendre en 30 Secondes)**

Imaginez que vous êtes **réalisateur** et que votre produit est un **film**.

- **L'AXE HORIZONTAL (de gauche à droite) = Votre SCÉNARIO.** C'est l'histoire que vous racontez, scène par scène, dans l'ordre._Exemple pour un film d'aventure :_ `Introduction du héros` → `Appel à l'aventure` → `Premier défi` → `Affrontement final` → `Retour triomphal`.
- **L'AXE VERTICAL (de haut en bas) = La RICHESSE de chaque scène.** Sous chaque scène, vous empilez les détails : les **éléments essentiels** (en haut) et les **effets spéciaux/ bonus** (en bas)._Exemple sous "Affrontement final" :_ En haut : `Le combat a lieu`. Au milieu : `Une musique épique`. En bas : `Une explosion géante en arrière-plan`.
- **LA LIGNE MAGIQUE = Votre PREMIER MONTAGE (le MVP).**
  Vous tracez une ligne horizontale. **Tout ce qui est AU-DESSUS de la ligne, c'est votre film sorti en salle.** Il est complet et captivant. Tout ce qui est en dessous, ce sont les scènes coupées ou les bonus pour le DVD.

**Traduisons cela dans votre projet.**

---

### **Exemple Concret : L'Application "Recettes & Cie"**

Vous développez une application de recettes de cuisine. Voici comment votre **liste plate** dans GitHub se transforme en **carte narrative**.

#### **ÉTAPE 1 : Votre "Scénario" Utilisateur (Axe Horizontal)**

Mettez-vous à la place de Julie, qui veut cuisiner un nouveau plat :

1. **Découvrir** une idée de recette.
2. **Consulter** les détails de la recette.
3. **Préparer** sa session de cuisine (liste de courses, ustensiles).
4. **Noter/Partager** son expérience.

Ces 4 étapes forment vos **colonnes**. C'est le parcours logique et incontournable.

#### **ÉTAPE 2 : Remplir les Colonnes (Axe Vertical)**

Pour chaque étape, vous empilez les User Stories **de la plus cruciale à la plus optionnelle**.

| Découvrir (Colonne 1)             | Consulter (Colonne 2)          | Préparer (Colonne 3)               | Noter/Partager (Colonne 4)     |
| :-------------------------------- | :----------------------------- | :--------------------------------- | :----------------------------- |
| **🔴 (HAUT) ESSENTIEL**           | **🔴 (HAUT) ESSENTIEL**        | **🔴 (HAUT) ESSENTIEL**            | **🔴 (HAUT) ESSENTIEL**        |
| Voir une liste de recettes        | Voir la liste des ingrédients  | Créer une liste de courses basique | Donner une note sur 5          |
| Filtrer par "plat principal"      | Voir les étapes de préparation | Cocher un ingrédient acheté        |                                |
| **🟡 (BAS) BONUS**                | **🟡 (BAS) BONUS**             | **🟡 (BAS) BONUS**                 | **🟡 (BAS) BONUS**             |
| Voir des recommandations perso    | Voir une vidéo de la recette   | Partager la liste avec un ami      | Écrire un commentaire détaillé |
| Lire un article de blog culinaire | Ajuster les portions           | Exporter la liste                  | Partager sur les réseaux       |

#### **ÉTAPE 3 : Tracer la Ligne de Votre MVP (Votre "Premier Montage")**

**Tracez une ligne horizontale qui passe sous les éléments ESSENTIELS de chaque colonne.**
**Votre MVP, c'est TOUT CE QUI EST AU-DESSUS DE CETTE LIGNE.**
C'est l'application minimale mais **parfaitement fonctionnelle** que vous livrerez en priorité. Les bonus viendront après.

**Pourquoi cette ligne est géniale ?**
Si quelqu'un propose d'ajouter "Partager sur les réseaux" (en bas de la colonne 4) au prochain sprint, vous pouvez répondre : _"C'est sous la ligne MVP. On doit d'abord finir de solidifier les étapes 'Consulter' et 'Préparer'. On le planifie pour plus tard."_

---

### **Votre Mission pour Cette Semaine (Sprint 3)**

**Objectif :** Tenir un atelier de **Story Mapping** dans votre équipe.

**Consignes :**

1. **Quand :** Lors de votre prochaine séance de **Backlog Refinement**.
2. **Matériel :** Utilisez **Miro**, **Figma/FigJam**, ou un simple **tableau avec des post-its**.
3. **Action :**
   - Identifiez les **3 à 5 grandes étapes** du parcours de VOTRE utilisateur (votre axe horizontal).
   - Placez **TOUTES** vos User Stories existantes sous l'étape correspondante, en les ordonnant par importance (essentiel → bonus).
   - **Tracez ensemble la ligne de votre MVP.** Soyez impitoyables !
4. **Livrable à Déposer :** Une **capture d'écran** ou une **photo** de votre Story Map finale, ajoutée à un fichier `STORY_MAP.md` dans votre repository GitHub.
5. **Bénéfice Immédiat :** Utilisez cette carte pour **choisir les stories de votre Sprint 4** de manière éclairée. Prenez ce qui est "au-dessus de la ligne" et dans la prochaine colonne logique à compléter.

---

### **Pourquoi Faire Ça MAINTENANT (Sprint 3) ?**

Parce que vous avez assez d'histoires pour que votre backlog devienne confus, mais il est encore temps de réorganiser votre plan de vol avant les sprints décisifs.

- **Pour le PO :** Vous aurez un outil visuel pour expliquer la priorité et défendre le scope du MVP.
- **Pour les Devs :** Vous verrez le **pourquoi** derrière chaque story et comment elles s'assemblent.
- **Pour le SM :** Vous faciliterez des planifications de sprint bien plus efficaces.
- **Pour l'Équipe :** Vous parlerez tous le même langage : celui de **l'expérience utilisateur à construire par étapes**.

**Cet outil est ce qui sépare une équipe qui "code des features" d'une équipe qui "délivre un produit avec une vision".**

# Ligne Magique du MVP : Application "Recettes & Cie"

Voici une illustration **concrète et visuelle** de la fameuse "ligne magique" qui définit votre MVP.

---

## EXEMPLE DE LIGNES CLAIREMENT DÉFINIES

```
[PARCOURS UTILISATEUR]   DÉCOUVRIR  →  CONSULTER  →  PRÉPARER  →  NOTER

[STACK VERTICAL]
                     ┌─────────────────────────────────────────────┐
AU-DESSUS            │                                             │
DE LA LIGNE          │  • Voir liste de recettes                   │← COLONNE 1
= VOTRE MVP          │  • Filtrer par "plat principal"             │
                     │                                             │
                     │  • Voir liste ingrédients                   │← COLONNE 2
                     │  • Voir étapes préparation                  │
                     │                                             │
                     │  • Créer liste courses basique              │← COLONNE 3
                     │  • Cocher ingrédient acheté                 │
                     │                                             │
                     │  • Donner une note sur 5                    │← COLONNE 4
─────────────────────┼─────────────────────────────────────────────┤ ← LA LIGNE MAGIQUE !
EN DESSOUS           │                                             │
DE LA LIGNE          │  • Recommendations personnalisées           │
= POUR PLUS TARD     │  • Articles de blog culinaire               │
                     │                                             │
                     │  • Vidéo tutoriel                           │
                     │  • Ajuster les portions automatiquement     │
                     │                                             │
                     │  • Partager liste avec ami                  │
                     │  • Exporter liste (PDF)                     │
                     │                                             │
                     │  • Commentaire détaillé                     │
                     │  • Partage sur réseaux sociaux              │
                     └─────────────────────────────────────────────┘
```

---

## CE QUE VOTRE MVP CONTIENT (AU-DESSUS DE LA LIGNE)

### **Colonne 1 : DÉCOUVRIR**

- **Voir une liste de recettes** (titre + image miniature)
- **Filtrer par catégorie** (entrée, plat, dessert)

### **Colonne 2 : CONSULTER**

- **Voir la liste complète des ingrédients**
- **Voir les étapes de préparation** (texte simple)

### **Colonne 3 : PRÉPARER**

- **Créer une liste de courses** automatique depuis la recette
- **Cocher manuellement** les ingrédients achetés

### **Colonne 4 : NOTER**

- **Donner une note globale** de 1 à 5 étoiles

---

## POURQUOI CETTE LIGNE EST-ELLE "MAGIQUE" ?

### **Scénario utilisateur COMPLET avec votre MVP :**

1. Julie ouvre l'app → **VOIT** des recettes de pâtes
2. Elle clique sur "Carbonara" → **CONSULTE** les ingrédients et étapes
3. Elle appuie sur "Liste de courses" → **PRÉPARE** sa session (liste générée)
4. Après avoir cuisiné, elle **NOTE** la recette 4/5

**L'expérience utilisateur est COMPLÈTE et UTILE !** Le problème central ("trouver et préparer une recette") est résolu.

---

## CE QUI RESTE EN DEHORS (EN DESSOUS DE LA LIGNE)

### **Pourquoi ces éléments attendront-ils ?**

| Élément                   | Pourquoi il est EN DESSOUS de la ligne                                      |
| ------------------------- | --------------------------------------------------------------------------- |
| **Vidéo tutoriel**        | L'essentiel (les étapes écrites) est déjà là. La vidéo est un "plus".       |
| **Partage sur réseaux**   | L'application fonctionne sans. C'est de la croissance, pas du coeur métier. |
| **Recommandations perso** | Nécessite des données d'usage que vous n'avez pas encore.                   |
| **Ajustement portions**   | Calcul complexe pour un gain marginal sur le MVP.                           |

---

## ANALOGIE DU FILM (REPRISE)

**Votre MVP (au-dessus de la ligne) = Le film sorti en salle**

- Histoire complète et cohérente
- Personnages bien développés
- Effets spéciaux de base
- **Le public ressort satisfait**

**Les bonus (en dessous) = Les scènes coupées au montage**

- Scènes de caractère supplémentaires
- Effets spéciaux "waouh"
- Cameos de célébrités
- **Le film fonctionnait très bien sans**

---

## IMPACT SUR VOS SPRINTS

### **Votre plan devient CLAIR :**

**Sprints 4-5 (MVP) :** Tout ce qui est **AU-DESSUS** de la ligne.
→ Vous livrez une application **utile et fonctionnelle**.

**Sprints 6-7 (Améliorations) :** Vous choisissez 1-2 éléments **EN DESSOUS** de la ligne, par colonne.
→ Ex: Ajouter la vidéo (colonne 2) ET le partage liste (colonne 3).

---

## VOTRE ARME SECRÈTE CONTRE LE "SCOPE CREEP"

**Quand on vous demande d'ajouter une feature :**
→ "Est-ce **au-dessus** ou **en dessous** de la ligne MVP ?"
→ "Si c'est en dessous, dans quelle release (2.0, 3.0) le planifions-nous ?"

**Exemple :**
_Client : "Et si on ajoutait un chatbot pour aider à choisir la recette ?"_
_VOUS : "Cela serait dans la colonne 'Découvrir', mais c'est clairement **en dessous de la ligne**. On le note pour la version 2.0, une fois qu'on aura validé que les bases marchent."_

---

## EXERCICE PRATIQUE POUR VOTRE ÉQUIPE

1. **Prenez vos User Stories actuelles**
2. **Classez-les dans les 4 colonnes** (Découvrir, Consulter, Préparer, Noter)
3. **Pour chaque colonne, posez-vous :**_"Si on ne livrait qu'UN SEUL élément de cette colonne, ce serait lequel ?"_ → Il va AU-DESSUS de la ligne.
   _"Qu'est-ce qui serait 'sympa d'avoir' mais pas indispensable ?"_ → Il va EN DESSOUS.
4. **Tracez VOTRE ligne** et prenez une photo !

**Rappel :** Une ligne bien placée est une ligne **impitoyable**. Si vous avez plus de 4-5 éléments par colonne au-dessus de la ligne, vous n'êtes probablement plus dans le "Minimum" de MVP.

---

**Cette ligne n'est pas une contrainte, c'est votre point de concentration.** Elle vous garantit de livrer l'essentiel, à temps, et de pouvoir en être fiers.
