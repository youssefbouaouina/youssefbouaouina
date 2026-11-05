# Youssef Bouaouina

**Élève ingénieur en cybersécurité — DFIR · Detection Engineering · DevSecOps**
Tunis, Tunisie · [Portfolio](https://youssefbouaouina.github.io/) · [LinkedIn](https://www.linkedin.com/in/youssef-bouaouina-93150330a) · [Email](mailto:youssefbouaouina82@gmail.com)

> 🎯 Recherche un **stage de fin d'études (PFE) de 6 mois à partir de janvier/février 2027** en ingénierie de détection, SOC/DFIR ou DevSecOps — mobilité internationale.

Je construis les outils des analystes : de la télémétrie brute d'un endpoint jusqu'au rapport d'investigation.

## Projets phares

### [ATOR DFIR](https://github.com/youssefbouaouina/ATOR) — plateforme d'investigation endpoint et de threat hunting
Stage DFIR chez NEXT STEP IT (juil.–sept. 2026) · [démo interactive](https://youssefbouaouina.github.io/portfolio/#ator)
- Agent de collecte Windows / Linux / Docker (9 modules, ordre de volatilité, manifestes SHA-256)
- API d'ingestion FastAPI (58 routes) : enrôlement, authentification par jeton, journal d'audit
- Détection : **16 règles Sigma → SQL (pySigma)**, 6 règles YARA, corrélation d'IOC, enrichissement MITRE ATT&CK hors ligne
- Rapports PDF, JSON, **STIX 2.1** et calque ATT&CK Navigator ; collecte Velociraptor à la demande
- **122 tests automatisés** sur mes modules, simulation de bout en bout 20/20

`Python` `FastAPI` `SQLite` `pySigma` `YARA` `MITRE ATT&CK` `STIX 2.1` `Velociraptor`

### [AD Detection Lab](https://github.com/youssefbouaouina/ad-detection-lab) — detection-as-code pour Active Directory · [démo](https://youssefbouaouina.github.io/ad-detection-lab/)
19 règles Sigma (DCSync, LSASS/SAM/NTDS, Kerberoasting, pass-the-hash, PsExec, WMI, désactivation des journaux) compilées en SQL avec pySigma et **mesurées sur 699 320 événements de 100 enregistrements d'attaques publics** : 73 % des détections attendues (86 % quand la télémétrie existe), vérité terrain figée avant le premier essai, 0 alerte bénigne sur 22 revues. CI : tests unitaires de détection + réévaluation + quality gate.

`Sigma` `pySigma` `SQLite` `MITRE ATT&CK` `Sysmon` `GitHub Actions`

### [Version 1 — DFIR & threat hunting framework](https://github.com/youssefbouaouina/dfir-threat-hunting-framework)
19 règles Sigma, backend conteneurisé, CI/CD GitHub Actions (ruff, validation des règles Sigma/YARA, publication de l'image Docker).

### [devopsNIDS — chaîne DevOps de bout en bout](https://github.com/youssefbouaouina/devopsNIDS)
Vagrant · Jenkins en 8 étapes (compilation → SonarQube → image Docker → déploiement et vérification Kubernetes sur Minikube) · Prometheus/Grafana · [démo](https://youssefbouaouina.github.io/portfolio/#devops)

### [MediTrack](https://github.com/youssefbouaouina/meditrack)
Django REST (JWT) + React/TypeScript : inventaire, OpenFDA, observance, interactions · [démo](https://youssefbouaouina.github.io/portfolio/#meditrack)

### Securify (académique)
Réseau segmenté (DMZ, honeypot, SOC, LAN) derrière pfSense/OPNsense ; SOC Wazuh, Shuffle, MISP, TheHive/Cortex.

## Stack
**Sécurité :** DFIR, threat hunting, Sigma, YARA, MITRE ATT&CK, STIX 2.1, Velociraptor, Wazuh, Shuffle, MISP, TheHive/Cortex, pfSense, OPNsense, Fortinet
**DevSecOps :** GitHub Actions, Jenkins, SonarQube, Docker, Kubernetes, Prometheus, Grafana
**Dev :** Python (FastAPI, Django), Java (Spring Boot), TypeScript (Angular, React), SQL

**Certifications :** Cisco CCNA 2 (SRWE) · Fortinet NSE 1, 2, 3
