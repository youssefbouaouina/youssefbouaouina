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

### [k8s-threat-detection-lab](https://github.com/youssefbouaouina/k8s-threat-detection-lab) — détection runtime dans Kubernetes
15 scénarios d'attaque scriptés contre Minikube, détectés par Falco 0.45.2 (eBPF) : **v1 3/15, v2 5/15 (33,3 %)** avec 5 règles custom, et **202,6 alertes bénignes/heure** mesurées sur une fenêtre de 15,4 min. Vérité terrain committée avant le premier essai, labo complet rejoué en CI, gate `v2 ≥ v1`.

`Falco` `Kubernetes` `Minikube` `Helm` `eBPF` `Python` `GitHub Actions`

### [secure-supply-chain-pipeline](https://github.com/youssefbouaouina/secure-supply-chain-pipeline) — chaîne DevSecOps mesurée
Image Spring Boot durcie de **477,2 à 221,0 Mio (−53,7 %)** et de **430 à 86 constats Grype (−80 %)** ; échecs Conftest/kube-linter de **16 à 0**. SBOM Syft, signature keyless cosign, provenance SLSA vérifiée et gate Grype sur les Critical corrigeables.

`Java 21` `Spring Boot` `Docker` `Syft` `Grype` `cosign` `SLSA` `Conftest` `GitHub Actions`

### [iac-misconfig-hunter](https://github.com/youssefbouaouina/iac-misconfig-hunter) — quatre scanners IaC comparés
**35 misconfigurations connues** (20 Terraform, 15 Kubernetes) évaluées avec Checkov, Trivy, KICS et kube-linter : **34/35 trouvées par au moins un scanner**, **14/14 constats ciblés supprimés** dans le module corrigé, total Checkov de **215 à 188**. Chaque match est traçable dans `matches.csv`.

`Terraform` `Kubernetes` `Checkov` `Trivy` `KICS` `kube-linter` `Python` `GitHub Actions`

### [kev-to-stix](https://github.com/youssefbouaouina/kev-to-stix) — CISA KEV vers STIX 2.1 · [démo](https://youssefbouaouina.github.io/kev-to-stix/)
Conversion quotidienne du catalogue CISA KEV : **1 768 entrées, 3 538 objets STIX 2.1 validés** (`stix2-validator`, sortie committée), identifiants UUIDv5 déterministes, **361 entrées liées à un ransomware** et 97 à un triage forensique. Workflow planifié et tableau de bord statique.

`Python` `STIX 2.1` `CISA KEV` `GitHub Actions` `GitHub Pages`

### [network-detection-lab](https://github.com/youssefbouaouina/network-detection-lab) — détection réseau Suricata + Zeek
Six scénarios d'attaque générés avec Scapy sur 10.10.0.0/24 : **6/6 détectés, 6 alertes malveillantes, 0 alerte sur la capture bénigne**. Règles Suricata écrites à la main et logs Zeek (conn, http, dns) évalués ensemble ; PCAP synthétiques pour une vérité terrain exacte et sans problème de licence.

`Scapy` `Suricata` `Zeek` `Python` `GitHub Actions`

### [windows-hardening-audit](https://github.com/youssefbouaouina/windows-hardening-audit) — audit de durcissement Windows · [rapport](https://youssefbouaouina.github.io/windows-hardening-audit/)
**40 contrôles CIS/ATT&CK** en PowerShell strictement lecture seule, score pondéré par sévérité et rapports JSON/Markdown/HTML. Sur un runner jetable : **13/40 (37,5) → 31/40 (75,7)**, **18 contrôles corrigés, aucune régression** ; 24 tests Pester et gate CI.

`PowerShell` `Pester` `CIS Benchmark` `MITRE ATT&CK` `GitHub Actions`

### [velociraptor-triage-artifacts](https://github.com/youssefbouaouina/velociraptor-triage-artifacts) — pack de triage DFIR
**12 artifacts VQL en lecture seule** (7 Windows, 5 Linux) pour la persistance, les services inscriptibles, les tâches encodées, les clés SSH, les binaires SUID et plus. Chaque test plante un marqueur, exécute le **vrai binaire Velociraptor 0.77.3** et exige sa présence : **7/7 Windows et 5/5 Linux** en CI.

`Velociraptor` `VQL` `YAML` `Python` `GitHub Actions`

### [Version 1 — DFIR & threat hunting framework](https://github.com/youssefbouaouina/dfir-threat-hunting-framework)
19 règles Sigma, backend conteneurisé, CI/CD GitHub Actions (ruff, validation des règles Sigma/YARA, publication de l'image Docker).

### [devopsNIDS — chaîne DevOps de bout en bout](https://github.com/youssefbouaouina/devopsNIDS)
Vagrant · Jenkins en 8 étapes (compilation → SonarQube → image Docker → déploiement et vérification Kubernetes sur Minikube) · Prometheus/Grafana · [démo](https://youssefbouaouina.github.io/portfolio/#devops)

### [MediTrack](https://github.com/youssefbouaouina/meditrack)
Django REST (JWT) + React/TypeScript : inventaire, OpenFDA, observance, interactions · [démo](https://youssefbouaouina.github.io/portfolio/#meditrack)

### Securify (académique)
Réseau segmenté (DMZ, honeypot, SOC, LAN) derrière pfSense/OPNsense ; SOC Wazuh, Shuffle, MISP, TheHive/Cortex.

## Stack
**Sécurité :** DFIR, threat hunting, Sigma, YARA, MITRE ATT&CK, STIX 2.1, Velociraptor (VQL), Falco, Suricata, Zeek, Wazuh, Shuffle, MISP, TheHive/Cortex, pfSense, OPNsense, Fortinet, durcissement Windows
**DevSecOps :** GitHub Actions, Jenkins, SonarQube, Docker, Kubernetes, Minikube, Trivy/Grype, Syft, cosign, SLSA, Checkov/KICS, Prometheus, Grafana
**Dev :** Python (FastAPI, Django), Java (Spring Boot), TypeScript (Angular, React), PowerShell/Pester, SQL

**Certifications :** Cisco CCNA 2 (SRWE) · Fortinet NSE 1, 2, 3
