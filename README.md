# PrésenceManager

Application Android de gestion des présences, développée avec Kotlin et XML dans le cadre de la formation en Développement Mobile à la CMC RSK – OFPPT.

## TP01 – Interface d'accueil

L'écran d'accueil contient le bouton « Commencer l'appel » qui ouvre le tableau de bord.

## TP02 – Tableau de bord

Le tableau de bord conserve ses quatre cartes : Groupes, Faire l'appel, Historique et Statistiques.

## TP03 – Gestion des événements

### Événements traités

- **Clic simple (`setOnClickListener`)** : le bouton « Commencer l'appel » ouvre le tableau de bord. Chaque carte ouvre son activité de destination : Groupes, Faire l'appel, Historique ou Statistiques.
- **Appui long (`setOnLongClickListener`)** : un appui long sur Groupes affiche « Groupes : sélectionner ou consulter les groupes ». Un appui long sur Faire l'appel affiche « Faire l'appel : démarrer une séance ». Ces actions affichent un Toast et ne déclenchent aucune navigation.
- **Double-clic (`GestureDetector` / `onDoubleTap`)** : deux appuis rapides sur l'image du profil affichent la boîte « À propos de PrésenceManager » avec la version 1.0.
- **Clic sur Version 1.0** : le texte de version de l'écran d'accueil et du tableau de bord ouvre la boîte « Informations du développeur ». Elle présente le nom du développeur et le lien GitHub cliquable.

### Pages accessibles depuis le tableau de bord

- `GroupesActivity` — `activity_groupes.xml`
- `AppelActivity` — `activity_appel.xml`
- `HistoriqueActivity` — `activity_historique.xml`
- `StatistiquesActivity` — `activity_statistiques.xml`

Chaque page affiche son titre et le texte « Fonctionnalité en cours de développement ».

## Technologies

- Kotlin
- XML
- Android Studio
- `Intent` et `startActivity`
- `OnClickListener` et `OnLongClickListener`
- `GestureDetector`
- `Toast` et `AlertDialog`
- `Linkify` et `LinkMovementMethod`

## Réalisé par

**Douae ELKHNICHA**  
CMC RSK – OFPPT | 2026–2027

GitHub : https://github.com/douaeelkhnicha/PresenceManager
