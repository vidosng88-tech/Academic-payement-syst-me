# Academic Payment System

Un système de gestion de paiement des frais académiques pour les étudiants, développé en Python.

## 📋 Description

Le **Academic Payment System** est une application complète permettant de :
- Gérer les frais académiques des étudiants
- Traiter les paiements de manière sécurisée
- Générer des reçus et factures
- Suivre l'historique des paiements
- Gérer les rappels de paiement

## 🎯 Objectifs

- Simplifier le processus de paiement des frais académiques
- Offrir une interface conviviale aux étudiants
- Garantir la sécurité des transactions
- Fournir des rapports détaillés aux administrateurs

## 🛠️ Stack Technologique

- **Langage** : Python 3.8+
- **Framework Web** : Django 4.2+
- **Base de données** : PostgreSQL/MySQL
- **Paiement** : Stripe, PayPal
- **API** : Django REST Framework

## 📁 Structure du Projet

```
Academic-payement-syst-me/
├── README.md
├── requirements.txt
├── .gitignore
├── .env.example
├── manage.py
├── config/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── payments/
│   ├── __init__.py
│   ├── models.py
│   ├── views.py
│   ├── serializers.py
│   ├── urls.py
│   └── admin.py
├── students/
│   ├── __init__.py
│   ├── models.py
│   ├── views.py
│   └── urls.py
├── tests/
├── migrations/
└── docs/
```

## 🚀 Installation

### Prérequis
- Python 3.8 ou supérieur
- pip (gestionnaire de paquets Python)
- virtualenv (recommandé)

### Étapes

1. **Cloner le repository**
```bash
git clone https://github.com/vidosng88-tech/Academic-payement-syst-me.git
cd Academic-payement-syst-me
```

2. **Créer un environnement virtuel**
```bash
python -m venv venv
source venv/bin/activate  # Sur Windows: venv\Scripts\activate
```

3. **Installer les dépendances**
```bash
pip install -r requirements.txt
```

4. **Configurer les variables d'environnement**
```bash
cp .env.example .env
# Éditer .env avec vos paramètres
```

5. **Initialiser la base de données**
```bash
python manage.py migrate
```

6. **Créer un superutilisateur**
```bash
python manage.py createsuperuser
```

7. **Lancer l'application**
```bash
python manage.py runserver
```

L'application sera accessible sur `http://localhost:8000`

## 📖 Documentation

- [Guide d'utilisation](docs/USAGE.md)
- [API Documentation](docs/API.md)
- [Architecture](docs/ARCHITECTURE.md)

## 🔐 Sécurité

- Authentification JWT pour les API
- Authentification SSL/TLS pour toutes les transactions
- Chiffrement des données sensibles
- Conformité PCI DSS pour les paiements
- Validation des entrées et protection contre les injections SQL

## 🧪 Tests

```bash
# Exécuter les tests
pytest

# Avec couverture
pytest --cov=payments --cov=students
```

## 🤝 Contribution

Les contributions sont bienvenues ! Pour contribuer :

1. Fork le project
2. Créer une branche feature (`git checkout -b feature/AmazingFeature`)
3. Commit vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrir une Pull Request

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## 👤 Auteur

**vidosng88-tech**

## 📞 Support

Pour des questions ou des problèmes :
- Ouvrir une [Issue](https://github.com/vidosng88-tech/Academic-payement-syst-me/issues)
- Consulter la [Discussion](https://github.com/vidosng88-tech/Academic-payement-syst-me/discussions)

---

**Dernière mise à jour** : Juin 2026
