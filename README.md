# Mpls-l3vpn-multisite-lab

# Conception et Déploiement d'une Architecture MPLS L3VPN Multi-Sites avec Interconnexion LAN Hétérogène

> Laboratoire réseau simulant l'interconnexion de trois sites clients hétérogènes (OSPF / EIGRP / Statique) via un backbone MPLS opérateur (L3VPN, MP-BGP, VRF), avec haute disponibilité LAN, VPN et ingénierie de trafic.

**Auteur :** Safae Kanbouh
**Année universitaire :** 2025 – 2026
**Outil de simulation :** GNS3
---

## 📖 Description

Les entreprises modernes multi-sites doivent interconnecter des réseaux locaux souvent hétérogènes, chaque site ayant été construit avec ses propres choix techniques (routage, commutation, sécurité). Pour répondre à ce besoin, les fournisseurs de services s'appuient sur la technologie **MPLS**, qui offre une connectivité **VPN de niveau 3 (L3VPN)** tout en mutualisant un backbone commun entre plusieurs clients, de façon isolée et sécurisée.

Ce laboratoire reproduit ce scénario avec **trois sites clients** (CE_A, CE_B, CE_C), chacun avec son propre LAN, ses VLANs et son propre protocole de routage interne (OSPF, EIGRP, statique), interconnectés via un backbone MPLS (routeurs P et PE) s'appuyant sur OSPF Area 0, LDP et MP-BGP.

## 🎯 Objectifs

- Concevoir et déployer une architecture réseau multi-sites complète, du LAN jusqu'au backbone MPLS
- Interconnecter des sites hétérogènes en préservant l'isolation et la sécurité du trafic
- Garantir la haute disponibilité et la performance du réseau à tous les niveaux (LAN, WAN, backbone)
- Développer une maîtrise pratique des technologies avancées de routage/commutation (MPLS, VPN, VRF, BGP, MPLS TE)

## 🛠️ Technologies utilisées

- **Commutation :** VLANs, VTP v3, Rapid-PVST (RSTP), EtherChannel (LACP / PAgP)
- **Routage inter-VLAN :** Router on a Stick (ROAS)
- **Routage interne CE :** OSPF, EIGRP, route statique
- **Backbone opérateur :** OSPF Area 0, LDP, MPLS
- **VPN opérateur :** MP-BGP, VRF (RD/RT), redistribution vers BGP
- **VPN site-à-site :** DMVPN
- **Ingénierie de trafic :** MPLS TE (tunnels RSVP-TE, extension OSPF TE)
- **Sécurité :** enable secret, sécurisation console, SSH v2 (clé RSA 2048)
- **Accès Internet** via le routeur P1

---
