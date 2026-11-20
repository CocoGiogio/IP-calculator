# 🌐 Calculateur IP (IPv4 & IPv6)

[![GitHub Pages](https://img.shields.io/badge/Démo_en_ligne-GitHub_Pages-2563eb?style=for-the-badge&logo=github)](https://cocogiogio.github.io/IP-calculator/)
[![PWA Ready](https://img.shields.io/badge/PWA-100%25_Hors_Ligne-10b981?style=for-the-badge&logo=pwa)](https://cocogiogio.github.io/IP-calculator/)
[![Zero Dependency](https://img.shields.io/badge/Stack-HTML_/_CSS_/_JS_Pur-f59e0b?style=for-the-badge)](#)

Application web progressive (PWA) légère, rapide et installable sur mobile permettant de calculer, découper et visualiser instantanément des sous-réseaux **IPv4** et **IPv6**.

👉 **Accéder à l'application :** [https://cocogiogio.github.io/IP-calculator/](https://cocogiogio.github.io/IP-calculator/)

---

## ✨ Fonctionnalités

* **Saisie universelle & intelligente** : Détection automatique du format saisi sans avoir à changer de formulaire :
  * Notation CIDR : `192.168.1.10/24` ou `2001:db8:85a3::1/64`
  * IPv4 + Masque direct : `10.10.0.5/255.255.254.0` ou `10.10.0.5 255.255.254.0`
  * IPv4 + Wildcard (ACL) : `172.16.40.1/0.0.0.255` ou `172.16.40.1 0.0.0.255`
  * IP seule : applique `/24` (IPv4) ou `/64` (IPv6) par défaut
* **Schéma réseau dynamique** :
  * Visualisation binaire des 32 bits (IPv4) ou 128 bits (IPv6) distinguant la partie **Réseau** de la partie **Hôtes**.
  * Identification automatique de la portée (Privé RFC 1918, CGNAT RFC 6598, APIPA, Public, ULA, Link-Local) et positionnement dans le super-réseau parent.
  * Navigation rapide vers le sous-réseau **précédent** ou **suivant**.
* **Curseur CIDR tactile** : Ajustement en temps réel du préfixe (`/0` à `/32` ou `/128`).
* **Copie en un clic** : Bouton de copie rapide sur chaque paramètre calculé (réseau, broadcast, plage d'hôtes, masque, wildcard).
* **Aide-mémoire IANA intégré** : Récapitulatif des plages d'adresses non routables.
* **Thème Sombre / Clair** : Bascule manuelle ou synchronisation automatique avec le thème système.

---

## 📱 Installation sur téléphone (Mode Application)

Grâce au *Service Worker* intégré, l'outil s'installe comme une application native et fonctionne **100 % hors ligne** (idéal en datacenter ou salle serveur).

* **iOS (Safari)** : Ouvrir [cocogiogio.github.io/IP-calculator](https://cocogiogio.github.io/IP-calculator/) → bouton **Partager** → **Sur l'écran d'accueil**.
* **Android (Chrome)** : Ouvrir [cocogiogio.github.
