# 🛡️ Simulateur de Phishing Éducatif

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Flask](https://img.shields.io/badge/Flask-3.0-green)
![Educational](https://img.shields.io/badge/Usage-Educational%20Only-orange)
![License](https://img.shields.io/badge/License-MIT-green)

**⚠️ OUTIL STRICTEMENT PÉDAGOGIQUE - USAGE ÉDUCATIF UNIQUEMENT ⚠️**

Simulateur de phishing conçu pour former et sensibiliser les utilisateurs aux dangers du phishing et du social engineering.

---

## 🎯 Objectif

Cet outil permet de :
- ✅ **Former** les employés à reconnaître les tentatives de phishing
- ✅ **Sensibiliser** aux techniques de social engineering
- ✅ **Tester** la vigilance en environnement contrôlé
- ✅ **Éduquer** sur les signaux d'alerte à repérer

## ⚠️ DISCLAIMER CRITIQUE

**LIRE ATTENTIVEMENT AVANT TOUTE UTILISATION**

- ❌ **NE JAMAIS** utiliser pour de vraies attaques
- ❌ **NE JAMAIS** utiliser sans consentement écrit
- ❌ **NE JAMAIS** capturer de vraies données
- ✅ **UNIQUEMENT** pour formation interne avec autorisation
- ⚖️ **Usage malveillant = ILLÉGAL** (jusqu'à 5 ans de prison)

Voir [DISCLAIMER.md](DISCLAIMER.md) pour les détails complets.

---

## ✨ Fonctionnalités

### 🎭 4 Scénarios de Simulation

1. **🏦 Alerte Bancaire**
   - Fausse alerte de sécurité bancaire
   - Urgence critique
   - 5 signaux d'alerte intégrés

2. **💻 Support Technique**
   - Fausse page de support Microsoft/Apple
   - Pop-up agressive
   - Timer de compte à rebours

3. **📱 Réseau Social**
   - Fausse page de connexion
   - Design approximatif
   - URL suspecte

4. **📦 Livraison Colis**
   - Faux suivi de colis
   - Demande de paiement
   - Expéditeur générique

### 🛡️ Signaux d'Alerte Éducatifs

Chaque scénario contient des signaux d'alerte visibles :
- URL suspectes (http://, domaines incorrects)
- Fautes d'orthographe volontaires
- Messages d'urgence excessive
- Timer de compte à rebours (fake)
- Design approximatif

### 📊 Fonctionnalités Pédagogiques

- **Détection volontaire** : Bouton "J'ai détecté du phishing !"
- **Rapports éducatifs** : Analyse détaillée après chaque test
- **Page de sensibilisation** : Explication des erreurs commises
- **Guide complet** : Conseils de prévention
- **Statistiques** : Taux de vigilance global

### 🔒 Sécurité des Données

- **AUCUNE donnée sensible collectée**
- Pas de stockage de mots de passe ou identifiants
- Rapports anonymes uniquement
- Redirection immédiate vers sensibilisation
- Aucune transmission de données externes

---

## 🚀 Installation

### Prérequis

- Python 3.8+
- pip

### Installation rapide

```bash
# Cloner le repository
git clone https://github.com/VAL-cyber-pentester/Phishing-Awareness-Tool.git
cd Phishing-Awareness-Tool

# Installer les dépendances
pip install -r requirements.txt

# Lancer l'application
python app.py
```

L'application sera accessible sur : **http://127.0.0.1:5000**

---

## 📖 Utilisation

### 1. Page d'Accueil

- Lire attentivement le **disclaimer éthique**
- Cocher la case de consentement
- Choisir un scénario de simulation

### 2. Scénario de Phishing

- Observer attentivement la page
- Repérer les signaux d'alerte
- **Option A** : Cliquer sur "J'ai détecté du phishing !" (✅ Vigilant)
- **Option B** : Remplir le formulaire (⚠️ Piégé)

### 3. Page de Sensibilisation

- Découvrir les signaux manqués
- Apprendre à reconnaître le phishing
- Consulter les recommandations
- Voir les statistiques globales

### 4. Guide de Prévention

- Consulter la page d'information
- Apprendre les 6 règles d'or
- Découvrir les types de phishing
- Obtenir des ressources officielles

---

## 📁 Structure du Projet

```
Phishing-Awareness-Tool/
├── app.py                      # Application Flask principale
├── config.py                   # Configuration et scénarios
├── requirements.txt            # Dépendances Python
├── README.md                   # Documentation
├── DISCLAIMER.md               # Avertissement éthique détaillé
├── templates/
│   ├── index.html             # Page d'accueil
│   ├── fake_login.html        # Fausse page de phishing
│   ├── awareness.html         # Page de sensibilisation
│   ├── report.html            # Rapport détaillé
│   └── info.html              # Guide de prévention
├── static/
│   ├── style.css              # Styles CSS
│   └── script.js              # JavaScript (minimal)
├── reports/                    # Rapports générés (anonymes)
└── data/                       # Données de configuration
```

---

## 🎓 Cas d'Usage Autorisés

### ✅ Utilisations Légitimes

- **Formation en entreprise** avec accord RH/DSI
- **Cours de cybersécurité** en établissement scolaire
- **Exercices de sensibilisation** avec encadrement professionnel
- **Tests de sécurité internes** avec autorisation écrite
- **Démonstrations pédagogiques** lors de conférences

### ❌ Utilisations INTERDITES

- Attaques contre personnes sans consentement
- Vol de données personnelles ou professionnelles
- Usurpation d'identité
- Fraude ou escroquerie
- Harcèlement ou intimidation
- Toute activité illégale

---

## 📊 Caractéristiques Techniques

### Backend
- **Flask 3.0** : Framework web Python
- **Session management** : Suivi des scénarios
- **Rapports JSON** : Génération de rapports anonymes

### Frontend
- **HTML5/CSS3** : Interface responsive
- **JavaScript vanilla** : Interactions dynamiques
- **Design moderne** : UX/UI claire et pédagogique

### Sécurité
- Aucune base de données sensible
- Pas de stockage de credentials
- Rapports anonymisés
- Disclaimers multiples

---

## 🛠️ Configuration

### Modifier les Scénarios

Éditer `config.py` pour ajouter/modifier des scénarios :

```python
SCENARIOS = {
    'custom': {
        'name': 'Mon Scénario',
        'description': 'Description du scénario',
        'target_site': 'Site Simulé',
        'urgency_level': 'Urgent',
        'red_flags': [
            'Signal 1',
            'Signal 2',
            # ...
        ]
    }
}
```

### Personnaliser le Disclaimer

Modifier `Config.DISCLAIMER` dans `config.py` pour adapter le message à votre organisation.

---

## 📈 Statistiques

L'application suit (de manière anonyme) :
- **Nombre de visites** total
- **Utilisateurs vigilants** (détection du phishing)
- **Utilisateurs piégés** (soumission du formulaire)
- **Taux de vigilance** global

Accès via : `/api/stats`

---

## 🔗 Ressources Officielles

- [ANSSI](https://www.ssi.gouv.fr/) - Agence Nationale de la Sécurité
- [Cybermalveillance.gouv.fr](https://www.cybermalveillance.gouv.fr/) - Assistance aux victimes
- [Signal Spam](https://www.signal-spam.fr/) - Signaler un spam/phishing
- [Phishing Initiative](https://www.phishing-initiative.fr/) - Signalement de phishing
- [CNIL](https://www.cnil.fr/) - Protection des données personnelles

---

## ⚖️ Aspects Légaux

### En France

**Articles 323-1 à 323-7 du Code pénal :**
- Accès frauduleux à un système informatique : **5 ans de prison + 150 000€ d'amende**
- Atteinte à l'intégrité des données : Peines aggravées

**RGPD (Règlement Général sur la Protection des Données) :**
- Violation : Amendes jusqu'à **20 millions d'euros** ou **4% du CA**

### Recommandations

1. **Obtenir une autorisation écrite** avant toute simulation
2. **Informer le RSSI/DSI** de l'organisation
3. **Documenter** le cadre pédagogique
4. **Conserver** les preuves de consentement
5. **Fournir un débriefing** après chaque simulation

---

## 🚀 Améliorations Futures

- [ ] Support multi-langues (EN, ES)
- [ ] Templates de scénarios personnalisables
- [ ] Export de rapports PDF
- [ ] Dashboard administrateur
- [ ] Intégration avec plateformes LMS
- [ ] Génération de certificats de formation
- [ ] Mode "campagne" pour tests planifiés

---

## 🤝 Contribution

Les contributions sont bienvenues **UNIQUEMENT** si elles respectent le caractère éducatif de l'outil.

**Ne proposez PAS :**
- Fonctionnalités facilitant de vraies attaques
- Méthodes de contournement de sécurité
- Techniques de capture de données réelles

**Proposez :**
- Nouveaux scénarios éducatifs
- Améliorations pédagogiques
- Traductions
- Documentation améliorée

---

## 📧 Contact

**Valérie ENAME**
- GitHub : [@VAL-cyber-pentester](https://github.com/VAL-cyber-pentester)
- LinkedIn : [Valérie ENAME](https://linkedin.com/in/valérie-ename-02ba7733a)

**Pour signaler un abus de cet outil :**
- [Cybermalveillance.gouv.fr](https://www.cybermalveillance.gouv.fr/)
- [Signal Spam](https://www.signal-spam.fr/)

---

## 📄 License

MIT License avec **restrictions éthiques strictes**.

L'usage commercial ou malveillant est **strictement interdit**.

Voir [LICENSE](LICENSE) pour les détails.

---

## 🙏 Remerciements

Projet créé dans le cadre d'un portfolio en cybersécurité pour démontrer :
- Compréhension des techniques de social engineering
- Capacité à créer des outils pédagogiques
- Engagement éthique en cybersécurité
- Compétences en développement web et Python

---

## ⚠️ RAPPEL FINAL

**CET OUTIL EST STRICTEMENT ÉDUCATIF**

- Ne l'utilisez JAMAIS pour nuire
- Respectez toujours les lois
- Obtenez toujours le consentement
- Soyez un acteur éthique de la cybersécurité

**"Avec de grands pouvoirs viennent de grandes responsabilités"**

---

**Dernière mise à jour : Décembre 2025**

⭐ **Si cet outil vous aide à sensibiliser, donnez-lui une étoile !**
