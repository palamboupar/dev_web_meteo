# MétéoFlash 🌦️

Projet Web universitaire – L2 Informatique – Semestre 4  
UE : Développement Web  
Année universitaire : 2024–2025  

## 👨‍💻 Membres de l’équipe

- BOUCHELAGHEM Ali  
- PALEOLOGOS Amaël  

## 🌐 URL du site

🔗 http://bouchelaghem.alwaysdata.net

## 📌 Objectif du projet

Créer un site web dynamique permettant à un utilisateur de :
- Consulter la météo actuelle d'une ville,
- Obtenir les prévisions sur plusieurs jours,
- Accéder à des informations techniques via API (JSON/XML),
- Visualiser les statistiques de consultation.

Le tout en proposant une navigation fluide, un affichage responsive, et un fonctionnement 100 % côté serveur (PHP + HTML + CSS).

---

## 🗺️ Fonctionnalités principales

- Navigation interactive par **carte HTML `<map>`** (région > département > ville)
- Affichage de la météo actuelle et des prévisions via **API JSON**
- Statistiques (nombre de consultations par ville) avec histogramme PHP en SVG
- Page "tech" avec intégration de :
  - L’image APOD du jour (NASA, JSON)
  - La géolocalisation par IP (GeoPlugin, XML)
- Stockage local :
  - Cookies : thème clair/sombre + ville consultée
  - CSV : historique de consultation côté serveur
- Thème clair/sombre configurable (avec persistance cookie)

---

## 🛠️ Technologies utilisées

| Type           | Outils / Langages |
|----------------|-------------------|
| Éditeur        | Visual Studio Code |
| Langages       | HTML5 / CSS3 / PHP 8 |
| Versioning     | Git + GitHub |
| Données météo  | [open-meteo.com](https://open-meteo.com/) (JSON) |
| API JSON       | [NASA APOD](https://api.nasa.gov) |
| API XML        | [GeoPlugin](http://www.geoplugin.com/) |
| Graphiques     | SVG généré via PHP |
| Stockage       | Fichier CSV / Cookies PHP |

---

## 📂 Arborescence simplifiée du projet

```text
meteoFlash/
├── index.php               # Page d’accueil avec image aléatoire
├── meteo.php               # Page d'affichage météo
├── stats.php               # Statistiques en SVG
├── tech.php                # Page test JSON / XML
├── header.inc.php          # Header commun
├── footer.inc.php          # Footer commun
├── data/
│   └── consultations.csv   # Enregistrement des villes consultées
├── assets/
│   └── img/photos/         # Dossier d’images pour accueil
