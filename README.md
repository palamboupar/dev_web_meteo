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
| Langages       | HTML / CSS / PHP |
| Versioning     | Git + GitHub |
| Données météo  | [weatherapi.com](https://www.weatherapi.com) (JSON) |
| API JSON       | [NASA APOD](https://api.nasa.gov) |
| API XML        | [GeoPlugin](http://www.geoplugin.com/) |
| Graphiques     | SVG généré via PHP |
| Stockage       | Fichier CSV / Cookies PHP |

---

## 📂 Arborescence simplifiée du projet

```text
MétéoFlash/
├── index.php               # Page d’accueil avec image aléatoire
├── meteo.php               # Page d'affichage météo
├── stats.php               # Statistiques 
├── tech.php                # Page test JSON / XML
├── plan.php                # Plan du site
├── include/
     └── header.inc.php     # Header commun
     └── footer.inc.php     # Footer commun
     └── function.inc.php   # Fonctions utilisées pour récupérer certaines données
     └── util.inc.php       # Permettant d'afficher le navigateur utilisé par l'utilisateur
├── css/
│   └── clair.css          # Thème clair 
│   └── sombre.css         # Thème sombre
├── ressources/
│   └── cities.csv                     # Stockage de toutes les villes de France 
│   └── v_departement_2024.csv         # Stockage de tous les départements de France
│   └── stats.csv                      # Stockage des villes les plus consultées 
├── td/	       
│   └── td1.php, td2.php, ...          # Ensemble des td effectués au fil du semestre 
├── images/                          
│   └── France.png, favicon.png, ...   # Les images utilisées pour le site
