---
title: Portfolio Jimmy PAULIN - Administrateur d’Infrastructures Sécurisées
---

# Jimmy PAULIN – Admin Infra & Sécurité (AIS)

En reconversion vers l’**administration d’infrastructures sécurisées**, je conçois et implémente des labs complets mêlant réseaux Cisco, virtualisation, firewall pfSense, VPN, bastions et homelab sur matériel réel.  
Ce portfolio regroupe une sélection de TP et projets réalisés en formation AIS (Simplon, Formatik) et en labs personnels.

- Localisation : Sorbiers (42) – proche Saint-Étienne / Lyon  
- Formation : AIS – Administrateur d’Infrastructures Sécurisées  
- Centres d’intérêt : réseaux Cisco, pfSense, VPN, bastions, virtualisation (Proxmox), cyber, scripts Python  

[GitHub](https://github.com/JiJiJuve) · [LinkedIn](TON_LIEN_LINKEDIN) · Contact : TON_EMAIL_PRO

---

## 1. Gros projets réseau & sécurité (Cisco)

### Infrastructure réseau multi‑sites haute disponibilité (Cisco Packet Tracer)

| Projet | Ce que j’ai fait | Lien |
|--------|-------------------|------|
| Infrastructure réseau d’entreprise haute dispo & sécurisée | Conception d’une infra complète siège + succursale + site Home : VLAN/VTP/trunks/EtherChannel/STP, routage inter‑VLAN sur switch L3, HSRP, DHCP central avec ip helper‑address, téléphonie IP (CME + TFTP), OSPF interne, NAT/PAT, serveur web publié, VPN IPsec site‑à‑site (Phase 1/2 + NONAT), VLAN 50 de gestion + SSH, Wi‑Fi succursale, démonstrations ICMP/HTTP/VoIP. | [TP détaillé](https://github.com/JiJiJuve/TP-Perso/tree/master/TP-Perso/TP-Infra-Haute-Dispo) |

---

## 2. Virtualisation & pfSense

| Projet | Ce que j’ai fait | Lien |
|--------|-------------------|------|
| Installation Proxmox VE + pfSense en lab virtualisé | Déploiement de Proxmox dans VirtualBox, vérification SHA256 de l’ISO, configuration réseau (bridge vmbr1), création d’une VM pfSense, configuration WAN/LAN, DHCP, accès à l’interface web depuis une VM Debian cliente, préparation d’un environnement pour futurs labs réseau/sécurité. | [TP détaillé](https://github.com/JiJiJuve/TP-Perso/tree/master/TP-Perso/Proxmox%2BPfsense) |
| VPN Client-to-Site avec pfSense & OpenVPN | Mise en place d’un pare‑feu pfSense, création d’un serveur OpenVPN SSL/TLS (CA, certificats serveur/client), règles firewall dédiées (DNS/HTTP/HTTPS/ICMP/OpenVPN), export des profils clients, installation du client OpenVPN sur une VM externe, tests d’accès sécurisé au LAN depuis l’extérieur (télétravail). | [TP détaillé](https://github.com/JiJiJuve/TP-Perso/tree/master/TP-Perso/Pfsense%2BOpenVPN) |

---

## 3. Bastions d’administration & accès sécurisé

| Projet | Ce que j’ai fait | Lien |
|--------|-------------------|------|
| Bastion d’administration Zero Trust avec Teleport | Étude comparative Teleport vs Apache Guacamole (sécurité, audit, types d’accès, déploiement), déploiement d’un bastion Teleport sur Debian, modèle Zero Trust avec certificats éphémères et MFA, gestion de ressources (serveurs) dans le bastion, connexions SSH depuis une VM cliente, traçabilité avancée des sessions (audit, relecture). | [TP Teleport](https://github.com/JiJiJuve/Simplon_Formation_AIS/blob/main/Bastion.md) |
| Bastion d’administration web avec Apache Guacamole | Déploiement d’un bastion Guacamole sur Debian (stack Tomcat + SQL), configuration d’utilisateurs et de connexions RDP/SSH, publication d’une VM Windows Server 2022 comme ressource administrable, accès RDP via navigateur depuis une VM cliente, tests de connexion et d’administration distante via le bastion. | [TP Guacamole](https://github.com/JiJiJuve/Simplon_Formation_AIS/blob/main/Guacamole.md) |

---

## 4. Lab réel sur matériel Cisco

| Projet | Ce que j’ai fait | Lien |
|--------|-------------------|------|
| Mise à jour IOS sur switch Cisco C2960X-24PS-L | Connexion console avec PuTTY, installation et configuration d’un serveur TFTP, téléchargement de la dernière image IOS, configuration d’une IP de management, tests de connectivité (ping PC / switch / serveur TFTP), transfert de la nouvelle image, configuration du boot, vérification de la version active, suppression de l’ancienne image et sauvegarde de la configuration. | Post LinkedIn (mise à jour du switch) |
| Récupération d’accès et config de base d’un routeur Cisco C892FSP-K9 | Passage en mode ROMMON pour récupération de mot de passe (confreg 0x2142 / 0x2102), boot sans config, récupération de la startup-config, modification des mots de passe, sauvegarde. Mise en place de la configuration de base : hostname, mots de passe console/VTY/enable secret, chiffrement des mots de passe, vérifications (show version, show interfaces, etc.). | Posts LinkedIn (ROMMON + config de base + lab réel routeur) |

*(Tu pourras remplacer “Post(s) LinkedIn …” par les URLs exactes de tes posts.)*

---

## 5. Réseau maison & projets en cours

Je construis progressivement un **réseau domestique avancé** dans ma nouvelle maison, en m’appuyant sur du matériel réel et des solutions open source :

- Baie de brassage en cours de déploiement avec routeur et switch Cisco, Wi‑Fi, segmentation prévue (VLAN utilisateurs, IoT/domotique, invités, management) et règles de sécurité (ACL).  
- Projet de **firewall dédié pfSense** : récupération de 3 vieux PC pour en faire une seule machine optimisée (mini‑serveur) qui prendra à terme le relais de la box FAI pour le NAT, le firewall et les VPN.  
- Mise en place prévue d’un **serveur Proxmox** pour héberger les VM (services internes, lab cyber), un futur NAS et d’autres briques d’infrastructure (surveillance, supervision, etc.).  

Ces projets viendront compléter les labs déjà réalisés en virtualisé (Proxmox + pfSense, VPN OpenVPN) par une mise en pratique sur matériel réel, dans un environnement proche d’une petite entreprise.

---

## 6. À venir

- Ajout de **scripts Python d’automatisation** (tri/renommage de fichiers, maintenance système, envoi d’e‑mails, etc.).  
- Intégration de **labs cybersécurité (TryHackMe / vulnérabilités Windows/AD)** documentés (contexte, exploitation, mitigation).  

Ce portfolio vise à montrer ma capacité à :
- concevoir une architecture réseau/sécurité cohérente,  
- documenter clairement mes labs,  
- et faire le lien entre formations AIS, labs personnels et homelab sur matériel réel.
