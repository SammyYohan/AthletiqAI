# ATHLETIQ AI — Coach de Fitness & Posture Intelligent avec IA Souveraine

<div align="center">

![Plateforme](https://img.shields.io/badge/Plateforme-Android_8.0%2B-3DDC84?logo=android&logoColor=white)
![Prix](https://img.shields.io/badge/Accès-100%25_Gratuit-2E7D32)
![Abonnement](https://img.shields.io/badge/Abonnement-Aucun-brightgreen)
![Confidentialité](https://img.shields.io/badge/Données-100%25_Locales_Souveraines-blue)
![Langues](https://img.shields.io/badge/Langues-FR_|_EN_|_ES_|_DE_|_IT_|_PT-orange)
[![Télécharger APK](https://img.shields.io/badge/Télécharger-APK_v1.0.0-C6F36A?logo=android&logoColor=black)](https://github.com/SammyYohan/AthletiqAI/releases/latest)

**L'application de musculation intelligente, souveraine et 100% gratuite qui analyse votre posture par caméra en temps réel, calibre vos programmes sur-mesure et respecte scrupuleusement votre vie privée.**

[English](README.md) • **Français** • [Español](README.es.md) • [Deutsch](README.de.md) • [Italiano](README.it.md) • [Português](README.pt.md)

[Téléchargement Direct](#-téléchargement--installation-android) • [Fonctionnalités Détaillées](#-toutes-les-fonctionnalités-détaillées) • [Le Mot de Sami Yohan](#-le-mot-du-créateur--sami-yohan) • [Soutien](#-soutenir-le-projet-ko-fi--paypal) • [Stack Technique](#-stack-technique)

</div>

---

## 💬 Le Mot du Créateur — Sami Yohan

> *« Bonjour à toutes et à tous,*
> 
> *Je m'appelle Sami Yohan. Je n'ai pas de fonds d'investissement derrière moi, ni de budget marketing. Je commence avec rien du tout en poche, juste des idées, de la passion et l'envie de créer des outils utiles et performants.*
> 
> *J'ai développé **ATHLETIQ AI** de A à Z depuis mon vieil ordinateur personnel. Mon objectif absolu est de mettre la technologie de pointe (vision par ordinateur, correction posturale biomécanique en temps réel, calcul métabolique sur-mesure) entre les mains de tous les passionnés de musculation et de remise en forme, sans aucune barrière financière.*
> 
> *Voilà pourquoi **ATHLETIQ AI est et restera 100% gratuite**. Aucun abonnement caché, aucun mur payant, aucune publicité intrusive.*
> 
> *Actuellement, l'application est **disponible uniquement sur Android**. Pourquoi ? Tout simplement parce que je n'ai pas encore assez d'argent pour m'acheter un MacBook (indispensable pour compiler avec Xcode) ni pour financer les frais récurrents du compte développeur Apple (99 $/an) ou encore les frais initiaux de publication sur le Google Play Store.*
> 
> *Si l'application vous plaît, qu'elle vous aide à progresser et à vous entraîner en toute sécurité, votre force et votre soutien via Ko-fi ou PayPal m'aident directement au quotidien pour faire grandir ce projet, publier officiellement sur le Play Store et, dès que possible, porter l'application sur iOS.*
> 
> *Merci du fond du cœur pour votre confiance ! »*
> 
> — **Sami Yohan**

---

## 📥 Téléchargement & Installation (Android)

L'application est distribuée sous forme de paquet APK signé prêt à l'emploi.

👉 **[Télécharger ATHLETIQ AI v1.0.0 (APK)](https://github.com/SammyYohan/AthletiqAI/releases/latest)**

### Comment l'installer en 3 étapes :
1. Téléchargez le fichier **`AthletiqAI-v1.0.0.apk`** depuis la page des [Releases](https://github.com/SammyYohan/AthletiqAI/releases/latest) sur votre téléphone Android.
2. Ouvrez le fichier téléchargé. Si Android vous demande d'autoriser l'installation d'applications provenant de sources inconnues (votre navigateur ou explorateur de fichiers), validez l'autorisation.
3. Lancez l'installation et profitez immédiatement de votre nouveau coach sans inscription obligatoire ni connexion requise !

> 📱 **Compatibilité** : Android 8.0 (Oreo, API 26) et versions supérieures (testé et optimisé jusqu'à Android 15 & 16). Fonctionne 100% hors-ligne.

---

## ✨ Toutes les Fonctionnalités Détaillées

### 1. 🎯 Onboarding & Profilage Biomécanique Complet
- **Parcours interactif pas à pas** : configuration intuitive de votre profil sans créer de compte en ligne.
- **Paramètres physiologiques** : âge, taille, poids (prise en charge du système Métrique kg/cm et Impérial lbs/in).
- **Objectif d'entraînement précis** : Hypertrophie, Force athlétique, Condition & Sèche, Technique & Posture, ou Reprise douce.
- **Matériel & Lieu d'entraînement** : Domicile au poids du corps, Matériel minimal (haltères, élastiques, barre de traction), ou Salle complète (barres olympiques, bancs, poulies, machines).
- **Personnalisation du volume** : fréquence réglable de **1 à 7 jours par semaine** et durée de séance personnalisable de **25 à 90 minutes**.
- **Ciblage des retards musculaires** : priorisez les zones à combler (Pectoraux, Épaules, Dos, Biceps, Triceps, Abdominaux, Quadriceps, Fessiers, Mollets).

### 2. 🧠 Moteur Algorithmique de Programmes (`ProgramEngine`)
- **Génération déterministe locale** : aucun aller-retour vers un serveur distant, génération instantanée et autonome.
- **Splits adaptés** : Full Body (1-3 j), Upper/Lower (4 j), Push/Pull/Legs (3-6 j), Arnold Split.
- **Priorisation anatomique des retards** : muscles cibles placés en début de séance avec intensité et volume optimisés.
- **Calibrage des répétitions & tempos** : 5-8 reps (Force), 8-12 reps (Hypertrophie), 12-15+ reps (Endurance).

### 3. 👁️ Coach Postural Caméra & IA Temps Réel (MediaPipe Tasks Vision)
- **Vision par ordinateur 100% embarquée** : propulsée par Google MediaPipe Tasks Vision (`pose_landmarker_lite.task`), s'exécutant directement sur le processeur/GPU de votre téléphone.
- **Tracking 3D de 33 repères anatomiques** : détection fine des genoux, hanches, épaules, coudes, poignets et chevilles.
- **Machine à états de répétition (`RepPhase`)** : détection automatique des phases (TOP, DESCENDING, BOTTOM, ASCENDING) avec validation stricte de l'amplitude.
- **Retour sonore temps réel (`ToneGenerator`)** : bip mélodieux de validation à chaque répétition propre, bip d'alerte spécifique si la forme se dégrade.
- **Prévention des blessures (Anti-Déchirure)** : surveillance du valgus du genou, contrôle du gainage lombo-pelvien et maintien de l'angle à 45° des coudes aux pompes.
- **Caméra avant/arrière & Mode manuel** : bascule selfie instantanée ou compteur manuel avec clicker sonore.

### 4. ⚡ Suivi de Séance en Direct (Active Workout)
- **Déroulé guidé série par série** avec affichage clair des charges et répétitions visées.
- **Ajustement instantané des charges** : boutons rapides `+ / - 2.5 kg` et `+ / - 5 kg`.
- **Sélecteur d'effort perçu RPE** : échelle de Borg graduée de 1 à 10 (RIR).
- **Minuteur de repos automatique** : déclenchement immédiat dès la série terminée, prolongation rapide `+30s` et sonnerie.
- **Substitution d'exercices à la volée** : remplacez un exercice en 1 clic par une variante équivalente.
- **Tolérance aux pannes** : sauvegarde automatique de la séance en cours (reprise instantanée).
- **Bilan de fin de séance complet** : durée nette, tonnage total déplacé (kg), séries complétées et XP gagné.

### 5. 📸 Body Scan Visuel & Analyse des Proportions
- **Captures multi-angles** : photo guidée ou enregistrement vidéo 360°.
- **Cartographie des 9 zones musculaires** : évaluation morphologique des Épaules, Pectoraux, Dos, Biceps, Triceps, Abdominaux, Quadriceps, Fessiers et Mollets.
- **Détection des points faibles** : scoring visuel (0-100) et calcul des deltas d'évolution.
- **Souveraineté absolue** : toutes les photos et vidéos restent exclusivement sur votre appareil. Aucun cloud.

### 6. 🥗 Calculateur Métabolique & Nutrition Avancée
- **BMR & TDEE** : calcul précis via la formule de Mifflin-St Jeor et ajustement selon la fréquence d'entraînement réelle.
- **Cible calorique automatisée** : Sèche (-350 kcal), Masse (+250 kcal), Force (+200 kcal), Maintien.
- **Macronutriments précis** : Protéines (1.7-2.1 g/kg), Lipides (~0.95 g/kg), Glucides équilibrés et hydratation personnalisée.
- **Conseils de récupération** : sommeil, repas pré/post-entraînement et repos nerveux.

### 7. 📈 Progrès, Historique & Records Personnels (PR)
- Graphiques interactifs sur 4, 8 et 12 semaines.
- Tableau des Records Personnels (1RM estimé et max de répétitions par exercice).
- Volume cumulé sur 30 jours et historique illimité de toutes les séances.

### 8. 🏆 Système de Gamification & Rangs d'Athlète
- 6 grades d'athlète évolutifs : Novice de la Fonte, Initié de la Charge, Pratiquant Hypertrophie, Sculpteur V-Taper, Maître de la Force, Titan Athlétique.

### 9. 📚 Bibliothèque d'Exercices Complète
- Fiches anatomiques complètes : consignes, erreurs fréquentes, variantes faciles/dures et substitutions.

### 10. 🌍 Multilingue & 🛡️ 100% Souverain
- 6 langues : Français, Anglais, Espagnol, Allemand, Italien, Portugais.
- 100% Hors-Ligne, zéro compte requis, zéro publicité, zéro pistage.

---

## 🛠️ Stack Technique

- **Langage** : Kotlin 2.1
- **UI Framework** : Android Jetpack Compose (Material Design 3)
- **Vision par Ordinateur & IA** : Google MediaPipe Tasks Vision (`tasks-vision:0.10.14`)
- **Pipeline Caméra** : AndroidX CameraX (Core, Camera2, Lifecycle, View)
- **Architecture** : MVVM réactif avec `StateFlow` et coroutines Kotlin
- **Persistance** : `LocalStore` souverain basé sur JSON typé
- **Cible Android** : `minSdk 26` (Android 8.0) • `targetSdk 36` (Android 16)

---

## ☕ Soutenir le Projet (Ko-fi & PayPal)

| Plateforme | Lien direct |
| :--- | :--- |
| ☕ **Ko-fi** | [ko-fi.com/sammyyohan](https://ko-fi.com/sammyyohan) |
| 💙 **PayPal** | [paypal.me/sammyyohan](https://paypal.me/sammyyohan) |

### À quoi servent les dons ?
1. **Frais de compte Google Play Console** (25 $) : pour publier l'application directement sur le Google Play Store.
2. **Financement d'un MacBook d'occasion** : matériel indispensable pour compiler sous Xcode afin de proposer ATHLETIQ AI sur iPhone.
3. **Licence Apple Developer Program** (99 $/an) : pour déployer l'application sur l'App Store iOS.

---

## 📄 Licence & Droits

Application conçue et développée par **Sami Yohan**.  
Tous droits réservés © 2026 Sami Yohan.
