# Car Sales Data Explorer 🚗📊

**Car Sales Data Explorer** est une application interactive construite avec **Streamlit**, permettant d'explorer, de filtrer et d'analyser un dataset de ventes de voitures. Elle intègre également un modèle génératif local (**Ollama**) pour répondre à des questions en langage naturel sur les données.

---

## 🚀 Fonctionnalités principales

### 🔍 **Exploration interactive des données**
- **Chargement CSV** : Importez facilement vos données de ventes de voitures à partir d’un fichier CSV.
- **Conversion automatique** :
  - `saledate` en format `datetime` (timezone naïve).
  - `make` en type `category` pour une meilleure performance.
- **Affichage dynamique** des données filtrées directement dans l'application.

---

### 🛠️ **Filtres personnalisés et options avancées**
- **Filtres dynamiques :**
  - Par plages de prix, fabricant, modèle ou autres colonnes.
  - Compatible avec les types de données numériques, catégoriques, objets et dates.
- **Agrégation des données :**
  - Regroupez par colonnes catégoriques avec des statistiques comme **moyenne**, **somme**, **min** et **max**.

---

### 🤖 **Intégration avec Ollama**
- **Questions dynamiques :** Posez des questions sur vos données en langage naturel (e.g., "Quel est le `sellingprice` pour l'année 2014 ?").
- **Vérification des réponses :** Les réponses générées par le modèle sont croisées avec les données du DataFrame.

---

## 🛠 Installation

### Prérequis
- **Python 3.8+**
- [Streamlit](https://streamlit.io) : Interface utilisateur interactive
- [Pandas](https://pandas.pydata.org) : Manipulation des données
- [Ollama](https://ollama.com) : Modèle génératif local pour les questions

### Instructions

1. Clonez le dépôt :
   ```bash
   git clone https://github.com/votre-repo/car-sales-explorer.git
   cd car-sales-explorer
   ```

2. Installez les dépendances :
   ```bash
   pip install -r requirements.txt
   ```

3. Assurez-vous que le modèle **Ollama** est installé et configuré sur votre machine :
   - Téléchargez et configurez Ollama depuis [le site officiel](https://ollama.com).

4. Lancez l’application Streamlit :
   ```bash
   streamlit run app.py
   ```

---

## ⚙️ Utilisation

### 1. Charger un fichier CSV
- Ajoutez un fichier CSV contenant les données de ventes de voitures dans le répertoire du projet (par défaut : `car_sales2.csv`).
- Exemple de colonnes :
  - `saledate` : Date de vente
  - `make` : Fabricant
  - `model` : Modèle
  - `sellingprice` : Prix de vente

### 2. Explorer les données dans Streamlit
- **Filtres :** Utilisez la barre latérale pour appliquer des filtres sur les prix, fabricants, modèles et autres colonnes.
- **Tri et regroupement :** Tri par colonnes ou regroupement avec statistiques agrégées.

### 3. Poser des questions avec Ollama
- Entrez une colonne cible et une condition pour poser des questions dynamiques (e.g., *Quelle est la valeur de `sellingprice` pour l'année 2014 ?*).
- Les réponses sont affichées et croisées avec le DataFrame pour validation.

### 4. Exporter les données filtrées
- Téléchargez les résultats filtrés sous forme de fichier CSV directement depuis l'application.

---

## 📂 Organisation du projet
- **`app.py`** : Fichier principal contenant le code de l'application Streamlit.
- **`requirements.txt`** : Liste des dépendances Python nécessaires.
- **`car_sales2.csv`** : Fichier d'exemple pour tester l'application (non inclus par défaut).

---

## 🤝 Contributeurs
- **Votre nom** : Développeur principal
- Contributions ouvertes aux pull requests !

---

## 📜 Licence
Ce projet est sous licence MIT. Consultez le fichier [LICENSE](LICENSE) pour plus d'informations.

