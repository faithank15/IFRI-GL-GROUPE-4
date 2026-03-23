# IFRI-GL-GROUPE-4

# TechDistrib SARL - Système de Gestion Intégré (ERP)

Ce projet consiste en la mise en place et la configuration d'une solution **Odoo v17.0** pour la gestion d'une entreprise de distribution de matériel informatique au Bénin. Il a été réalisé dans le cadre de la Licence 2 en **Génie Logiciel** à l'**IFRI (Université d'Abomey-Calavi)**.

## Présentation du Projet
**TechDistrib SARL** est une plateforme permettant de centraliser les flux de vente, de stock, de comptabilité et de ressources humaines. L'objectif est d'assurer la traçabilité complète des opérations, de la commande client jusqu'à l'enregistrement comptable conforme aux normes locales.

###  Acteurs et Rôles Configurés
Le système repose sur une gestion stricte des droits d'accès pour garantir la sécurité des données :
* **Administrateur :** Supervision technique et configuration globale.
* **Responsable Commercial :** Gestion du cycle de vente (Devis, Bons de commande).
* **Gestionnaire de stock :** Contrôle des mouvements de stock (Réceptions, Livraisons).
* **Comptable :** Facturation, paiements et écritures (Norme SYSCOHADA).
* **Responsable RH :** Gestion des fiches employés et des structures organisationnelles.

---

## Architecture Technique
La solution est entièrement conteneurisée, ce qui facilite son déploiement sur n'importe quel environnement (Windows, Linux, macOS).

* **Application :** Odoo 17.0 (Community Edition)
* **Base de données :** PostgreSQL 15
* **Infrastructure :** Docker & Docker Compose
* **Réseau :** Exposition du port `8069` pour un accès collaboratif en réseau local.

---

## Installation et Lancement

### Prérequis
* [Docker Desktop](https://www.docker.com/products/docker-desktop/) opérationnel.
* Accès à un terminal (PowerShell ou Bash).

### Étapes de démarrage
1. **Cloner le dépôt :**
   ```bash
   git clone [https://github.com/Krisaff7/techdistrib-odoo.git](https://github.com/Krisaff7/techdistrib-odoo.git)
   cd techdistrib-odoo

2. **Démarrage :** Ouvrez un terminal dans le dossier racine et tapez :
   ```bash
   docker-compose up -d

3. ** Acces Local au systeme : ** Si vous travaillez directement sur l'ordinateur où Docker est installé :
   ```bash
   http://localhost:8069

4.** Acces Multi-poste : ** Si vous travaillez directement sur l'ordinateur où Docker est installé :
   ```bash
   http://<ADRESSE_IPv4_DU_SERVEUR>:8069

