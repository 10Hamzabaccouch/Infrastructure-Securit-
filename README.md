# Infrastructure Multi-Service Sécurisée
Système d'infrastructure Linux complet avec 7 services sécurisés et 4 scripts Python d'automatisation
##  Objectifs
Infrastructure multi-service fonctionnelle
- Démonstration de sécurité et hardening
- Portfolio technique personnel

## ✅ Services implémentés

- **Apache** - Serveur web HTTP/HTTPS avec certificat SSL auto-signé
- **SSH** - Sécurisé sur port 2222 (root login désactivé)
- **DNS** - BIND9 pour résolution de domaines
- **Mail** - Postfix (SMTP) + Dovecot (IMAP/POP3)
- **FTP** - vsftpd pour transferts de fichiers
- **DHCP** - Allocation d'adresses IP
- **UFW** - Firewall avec règles configurées

## 🐍 Scripts Python

1. **monitor.py** - Surveillance en temps réel des services
2. **create_user.py** - Création automatique d'utilisateurs système
3. **backup.py** - Sauvegarde des configurations (tar.gz)
4. **chatbot.py** - Chatbot interactif avec API Google Gemini

## 🔒 Sécurité implémentée

- Certificat SSL/TLS auto-signé pour HTTPS
- SSH durci (port 2222, PermitRootLogin no)
- Firewall UFW avec règles strictes
- Validation des inputs Python
- Logs de sécurité et audit trail
- Protection contre brute force SSH

## 🎬 Démonstration d'attaque

Le projet inclut une démonstration fonctionnelle d'attaque et de défense :

- Scan de ports (nmap) depuis VM attaquant
- Tentative de brute force SSH (hydra)
- **Résultat** : UFW bloque automatiquement
- Logs enregistrant les 10+ tentatives échouées
- **Conclusion** : Infrastructure sécurisée ✓

## 🏗️ Configuration Lab

### Architecture de test

- **VM Serveur** : 192.168.50.1 (Ubuntu Server 24.04)
- **VM Attaquant** : 192.168.50.3 (Ubuntu)
- **Client** : 192.168.50.100 (Windows 7)
- **Réseau** : VirtualBox Internal Network

*Note: Ces IPs sont spécifiques au lab local. À adapter selon votre environnement.*

## 🚀 Installation

```bash
# Cloner le repo
git clone https://github.com/10Hamzabaccouch/Infrastructure-Securité.git
cd Infrastructure-Securité

# Installer les dépendances Python
cd Scripts
python3 -m venv venv
source venv/bin/activate
pip install google-generativeai requests

# Lancer les scripts
python3 monitor.py
python3 create_user.py
python3 backup.py
python3 chatbot.py
```

## 📊 Résultats obtenus

- ✓ 100% des services opérationnels
- ✓ Toutes les tentatives d'attaque bloquées
- ✓ 4 scripts Python testés et validés
- ✓ Logs de sécurité complets
- ✓ Documentation exhaustive

## 📁 Structure du projet


## 🎓 Apprentissages clés

- Configuration de services Linux critiques
- Hardening et sécurité système
- Automatisation avec Python
- Démonstration de concepts de sécurité
- Gestion complète de projet technique

## 👤 Auteur

**Hamza** - Étudiant Licence 3 Informatique

## 📝 Licence

MIT License - Libre d'utilisation et de modification

**Statut** : Projet terminé et testé ✓
**Date** : Août 2026
