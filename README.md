#Lab2 💰 HabitationAndroid — Calcul d'Impôts Locaux

Application Android développée dans le cadre d'un lab de développement mobile, permettant de calculer les impôts locaux d'un bien immobilier à partir des informations du propriétaire.

---

## 🎬 Démonstration



https://github.com/user-attachments/assets/9a083890-2ac7-4b72-935c-3d8a0aa0073c



> Remplace le lien ci-dessus par l'URL réelle de ta vidéo après l'avoir uploadée sur GitHub.

---

## ✨ Fonctionnalités

- Saisie des informations du propriétaire (nom et adresse)
- Saisie des caractéristiques du bien (surface en m², nombre de pièces)
- Indication de la présence d'une piscine via une case à cocher
- Validation des champs avant le calcul
- Affichage du résultat détaillé dans une boîte de dialogue (AlertDialog)
- Gestion des erreurs de saisie (champs vides, valeurs non numériques)

---

## 🧮 Formule de calcul

```
Impôt de base  = surface (m²) × 2
Supplément     = (nombre de pièces × 50) + (100 DH si piscine)

Total (DH)     = Impôt de base + Supplément
```

**Exemple :**
- Surface : 100 m² → 200 DH
- 3 pièces → 150 DH
- Piscine → 100 DH
- **Total : 450 DH**

---

## 🖥️ Interface utilisateur

| Champ | Type de vue |
|---|---|
| Nom du propriétaire | `EditText` |
| Adresse | `EditText` |
| Surface (m²) | `EditText` (numérique) |
| Nombre de pièces | `EditText` (entier) |
| Piscine | `CheckBox` |
| Calculer | `MaterialButton` |
| Résultat | `AlertDialog` (popup) |

---

## 🗂️ Structure du projet

```
app/
├── src/
│   └── main/
│       ├── java/com/example/habitationandroid/
│       │   └── MainActivity.java
│       └── res/
│           └── layout/
│               └── activity_main.xml
└── AndroidManifest.xml
```

---

## 📦 Dépendances

```gradle
implementation 'com.google.android.material:material:1.x.x'
```

> `MaterialButton` est utilisé pour le bouton de calcul — nécessite la librairie **Material Design**.

---

## 🚀 Installation & lancement

1. Cloner le projet et l'ouvrir dans **Android Studio**
2. Lancer un émulateur ou connecter un appareil Android
3. Cliquer sur **Run ▶**
4. Remplir les champs et appuyer sur **Calculer**

---

## 🛠️ Technologies

- **Java** — Logique métier et gestion des événements
- **XML** — Mise en page de l'interface
- **Material Design** — Composants UI modernes (`MaterialButton`)
- **AlertDialog** — Affichage du résultat en popup
- **Android Studio** — Environnement de développement

---

## 👩‍💻 Auteure

Développé par **Kaoutar** dans le cadre d'un lab Android.
