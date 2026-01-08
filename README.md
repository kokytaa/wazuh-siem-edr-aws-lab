# Atelier Sécurité des Endpoints et Supervision SIEM – Wazuh

## 📌 Description
Ce projet présente la mise en œuvre d’une plateforme complète de sécurité basée sur **Wazuh (SIEM + EDR)**,
déployée dans un environnement **AWS Learner Lab**, couvrant des systèmes **Linux et Windows**.

L’objectif est de démontrer le fonctionnement d’un **SOC moderne**, capable de collecter, corréler
et analyser des événements de sécurité en temps réel.

---

## 🏗️ Architecture du Lab
- EC2 Ubuntu : Wazuh All-in-One (Manager, Indexer, Dashboard)
- EC2 Ubuntu : Client Linux (Wazuh Agent)
- EC2 Windows Server : Client Windows (Wazuh Agent + option Sysmon)
- VPC AWS sécurisé avec Security Groups dédiés

Les schémas sont disponibles dans : `docs/architecture/`

---

## 🔐 Technologies utilisées
- Wazuh SIEM & EDR
- AWS EC2 / VPC / Security Groups
- Ubuntu 22.04 LTS
- Windows Server
- Sysmon (optionnel)

---

## ⚙️ Installation & Déploiement
Les étapes détaillées sont disponibles dans le dossier `installation/` :
- Création des instances AWS
- Configuration réseau et Security Groups
- Installation du serveur Wazuh
- Enrôlement des agents Linux et Windows

---

## 🧪 Scénarios SIEM & EDR
Les démonstrations incluent :
- Tentatives SSH échouées (Linux)
- Élévation de privilèges
- Modification de fichiers sensibles (FIM)
- Échecs de connexion Windows
- Création d’utilisateurs et gestion des groupes

Voir : `demo/siem-edr-scenarios.md`

---

## 📊 Résultats
Les preuves de fonctionnement sont disponibles dans `docs/screenshots/` :
- Agents actifs
- Alertes Linux
- Alertes Windows
- Événements IAM

---

## 🎯 Objectifs pédagogiques
- Comprendre le rôle du SIEM et de l’EDR
- Mettre en place une supervision de sécurité multi-OS
- Initier aux concepts de threat hunting et SOC

---

## 👤 Réalisé par
- Nom : Kawtar Khallouf
- Filière :Big Data
- Année : 2026–2027
