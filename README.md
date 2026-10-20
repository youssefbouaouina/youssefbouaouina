# Youssef Bouaouina

**Étudiant en ingénierie cybersécurité & DevOps**
DFIR · SOC · Detection Engineering · CI/CD

Tunis, Tunisie · [Email](mailto:youssefbouaouina82@gmail.com) · [LinkedIn](https://www.linkedin.com/in/youssef-bouaouina-93150330a)

---

Étudiant en cycle d'ingénieur à **ESPRIT**, spécialisé en cybersécurité et DevOps. Je développe des
outils concrets pour l'investigation endpoint, l'ingénierie de détection et la réponse à incident, et
j'automatise le build, les tests et le déploiement des applications sur lesquelles je travaille.

Je recherche actuellement un **stage ou un premier poste** en DFIR / SOC / detection engineering ou DevOps.

**Démos interactives :** [portfolio](https://youssefbouaouina.github.io/portfolio/) — ATOR, MediTrack et pipeline CI/CD, sans installation ni compte.

## Projets phares

### [ATOR — Framework d'investigation endpoint et de threat hunting](https://github.com/youssefbouaouina/ATOR)

Plateforme DFIR légère pour hôtes Windows, Linux et Docker, développée pendant mon stage en DFIR.

**Démo navigateur :** [rejouer une investigation ATOR](https://youssefbouaouina.github.io/portfolio/#ator) — 6 détections, 3 endpoints et une chaîne ATT&CK de 5 étapes.

- Architecture en six couches : collecteur portable, API d'ingestion FastAPI, stockage SQLite, moteur
  de détection, enrichissement MITRE ATT&CK et rapports/tableau de bord.
- Détection avec **YARA**, **règles Sigma compilées en SQL** via pySigma et corrélation d'IOC avec des
  watchlists locales.
- Enrichissement hors ligne **MITRE ATT&CK** (tactiques, techniques, sources de données) et
  reconstruction de la chaîne d'attaque.
- Rapports prêts pour l'investigateur aux formats **PDF, JSON, STIX 2.1 et ATT&CK Navigator**.
- Workflow de containment des endpoints et collecte forensic à la demande avec **Velociraptor**.
- Validée par 34/34 tests unitaires et d'intégration et une simulation end-to-end de 20/20.

`Python` `FastAPI` `SQLite` `YARA` `Sigma` `MITRE ATT&CK` `Velociraptor` `STIX 2.1` `Jinja2` `Chart.js`

### [MediTrack — Plateforme de gestion des médicaments](https://github.com/youssefbouaouina/meditrack)

Application full-stack de gestion des médicaments : inventaire, observance et contrôle des interactions.

**Démo navigateur :** [explorer MediTrack](https://youssefbouaouina.github.io/portfolio/#meditrack) — données d'exemple, stockage local.

- Backend Django REST avec authentification JWT et frontend React + TypeScript.
- Inventaire des médicaments, scan de codes-barres via OpenFDA, calendrier hebdomadaire d'observance,
  contrôle des interactions et alertes de stock faible.

`Django` `DRF` `React` `TypeScript` `Vite` `TailwindCSS`

### [devopsNIDS](https://github.com/youssefbouaouina/devopsNIDS)

Service Java/Spring Boot conteneurisé avec Docker et livré via un pipeline Jenkins.

**Démo navigateur :** [exécuter le pipeline](https://youssefbouaouina.github.io/portfolio/#devops) — succès et échec de test simulés.

`Java` `Spring Boot` `Docker` `Jenkins`

### Travaux académiques sélectionnés

- **Securify — Sécurité réseau par zones et architecture SOC :** réseau segmenté avec zones DMZ,
  honeypot, SOC et LAN ; pare-feux pfSense/OPNsense ; Wazuh (SIEM), Shuffle (SOAR), MISP (threat
  intelligence) et TheHive/Cortex (réponse à incident) ; simulations d'attaques et analyse de la détection.
- **Pipeline CI/CD pour une application Spring Boot :** pipeline Jenkins avec intégration GitHub,
  quality gates SonarQube, Docker, déploiement Kubernetes et supervision Prometheus/Grafana.

`Wazuh` `Shuffle` `MISP` `TheHive` `Cortex` `pfSense` `OPNsense` `Jenkins` `SonarQube` `Kubernetes`

## Stack technique

**Langages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**Cybersécurité**

![DFIR](https://img.shields.io/badge/DFIR-1F3864?style=flat-square)
![Threat Hunting](https://img.shields.io/badge/Threat_Hunting-1F3864?style=flat-square)
![Detection Engineering](https://img.shields.io/badge/Detection_Engineering-1F3864?style=flat-square)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-C00000?style=flat-square)
![YARA](https://img.shields.io/badge/YARA-2E8B57?style=flat-square)
![Sigma](https://img.shields.io/badge/Sigma-4B0082?style=flat-square)
![Wazuh](https://img.shields.io/badge/Wazuh-005571?style=flat-square)
![MISP](https://img.shields.io/badge/MISP-2C3E50?style=flat-square)
![Velociraptor](https://img.shields.io/badge/Velociraptor-333333?style=flat-square)
![Fortinet](https://img.shields.io/badge/Fortinet-DA291C?style=flat-square&logo=fortinet&logoColor=white)

**Backend**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Symfony](https://img.shields.io/badge/Symfony-000000?style=flat-square&logo=symfony&logoColor=white)

**DevOps & Cloud**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

## Certifications

- Cisco CCNA 2 — Switching, Routing and Wireless Essentials (SRWE) — Cisco Networking Academy
- [Fortinet NSE 1 — Network Security Associate](https://training.fortinet.com/admin/tool/certificate/index.php) — Fortinet · ID `5116367382YB`
- [Fortinet NSE 2 — Network Security Associate](https://training.fortinet.com/admin/tool/certificate/index.php) — Fortinet · ID `5048210791YB`
- [Fortinet NSE 3 — Network Security Associate](https://training.fortinet.com/admin/tool/certificate/index.php) — Fortinet · ID `2083836175YB`

Vérification Fortinet : [training.fortinet.com](https://training.fortinet.com/admin/tool/certificate/index.php) — saisir l'ID du certificat.

## Contact

- Email : [youssefbouaouina82@gmail.com](mailto:youssefbouaouina82@gmail.com)
- LinkedIn : [youssef-bouaouina-93150330a](https://www.linkedin.com/in/youssef-bouaouina-93150330a)
- GitHub : [youssefbouaouina](https://github.com/youssefbouaouina)
