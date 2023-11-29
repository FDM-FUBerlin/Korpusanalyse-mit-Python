<p align="center">
  <a href="" rel="noopener">
 <img width=300px height=300px src="data/04_images/frog-wordcloud.png" alt="Project logo"></a>
</p>

<h1 align="center">Einführung in die Korpusanalyse mit Python</h1>

<p align="center">Heinz-Alexander Fütterer (Freie Universität Berlin)</p>
<p align="center">Susanne Haaf (Berlin-Brandenburgische Akademie der Wissenschaften)</p>


<p align="center">
  <a href="https://mybinder.org/v2/gh/FDM-FUBerlin/Korpusanalyse-mit-Python.git/HEAD">
    <img src="https://mybinder.org/badge_logo.svg" alt="Binder">
  </a>
</p>

## 🧐 About <a name="about"></a>

Dieser Einführungskurs zur Programmiersprache Python für die Datenauswertung und Korpusanalyse richtet sich an Teilnehmer:innen mit grundlegenden Vorkenntnissen im Bereich der Programmierung allgemein. In einem ersten Teil werden Grundlagen von Python und der Textverarbeitung mit Python behandelt und erste Auswertungen mit dem NLTK (Natural Language Toolkit) unternommen.

Der zweite Teil geht auf die Möglichkeiten der individuellen Auswertung annotierter Korpora (des Deutschen), vom Dateninput über statistische Analysen bis hin zur Visualisierung von Ergebnissen ein.

Diese Veranstaltung ist Teil der Reihe "D4T4 L1T3R4CY".

## 📚 Inhalte <a name="contents"></a>

- Python: Einführung & grundlegende Konzepte 
- Methoden zum Einlesen, Aufbereiten & (statistischen) Analysieren von Textdaten
- nützliche Bibliotheken: Pandas, Matplotlib, NumPy, SciPy, NLTK
- Jupyter Notebooks/Jupyter Lab
- Fehlermeldungen & Dokumentation

### Lernziele
- Verständnis für den Einsatz und das Potenzial von Python für die Textverarbeitung und Korpusanalyse
- Einführung zum Einsatz einschlägiger Bibliotheken
- Befähigung zum Umgang mit Fehlermeldungen und sonstigen Problemen

### Agenda




## 🏁 Getting Started <a name="getting_started"></a>

Alle für die Teilnahme am Workshop bzw. zum Nacharbeiten benötigten Informationen und Noteboooks sind in diesem Git-Repository enthalten.

### Voraussetzungen

Eine aktuelle Python-Version (>= Python 3.8) wird benötigt. Zur Installation siehe:
- https://www.python.org/downloads/
- https://wiki.python.org/moin/BeginnersGuide/Download

### Installation
Zunächst dieses Git-Repository als ZIP herunterladen und entpacken bzw. mit `git clone` klonen:

```console
git clone https://github.com/FDM-FUBerlin/Korpusanalyse-mit-Python.git
cd Korpusanalyse-mit-Python/
```

Die benötigten Bibliotheken lassen sich am einfachsten mit `pip` installieren.

#### Unter Windows
```console
python -m venv .venv
.venv\Scripts\activate
(.venv) pip install --upgrade pip
(.venv) pip install .
(.venv) python -m nltk.downloader punkt stopwords
```

#### Unter Linux/MacOS
```console
python -m venv .venv
source .venv/bin/activate
(.venv) pip install --upgrade pip
(.venv) pip install .
(.venv) python -m nltk.downloader punkt stopwords
```

Wenn ebenfalls `JupyterLab` installiert werden soll:

```console
(.venv) pip install ".[jupyter]"
```

## 🎈 Nutzung <a name="usage"></a>
Die Jupyter-Notebooks in `notebooks/` sind am besten mit `JupyterLab` auszuführen:

```console
(.venv) jupyter lab
```

Alle Notebooks können mit folgendem Befehl ausgeführt werden.

```console
(.venv) jupyter nbconvert --to notebook --execute --inplace --allow-errors notebooks/*.ipynb
```
Daraufhin werden die benötigten Textdaten heruntergeladen und aufbereitet.

## ⛏️ Bibliotheken <a name="built_using"></a>
- [NLTK](https://www.nltk.org/) - Natural Language Processing
- [pandas](https://pandas.pydata.org/) - Datenanalyse
- [requests](https://docs.python-requests.org/en/latest/) - Web
- [seaborn](https://seaborn.pydata.org/) - Visualierungen
- [stylecloud](https://github.com/minimaxir/stylecloud) - Visualierungen
- [HanTa](https://github.com/wartaal/HanTa) - Natural Language Processing
- uvm.

## ✍️ Autor:innen <a name="authors"></a>
- Heinz-Alexander Fütterer
- Susanne Haaf

## 📜 Lizenz <a name="license"></a>
Die Inhalte dieses Git-Repositories sind unter einer [Creative Commons Namensnennung 4.0 International Lizenz](https://creativecommons.org/licenses/by/4.0/) lizenziert.

[![License](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by.svg)](https://creativecommons.org/licenses/by/4.0/)

## 🎉 Danksagung <a name="acknowledgement"></a>
- Die Materialien basieren auf [Textarbeit-mit-Python](https://github.com/FDM-FUBerlin/Textarbeit-mit-Python) (2022, Heinz-Alexander Fütterer und Selina Reinhard)
- README basiert auf [README_TEMPLATES/Standard.md](https://github.com/kylelobo/The-Documentation-Compendium/blob/master/en/README_TEMPLATES/Standard.md)
- Die Textanalysen basieren auf Märchenkorpus (lizenziert unter CC BY 3.0): Walter, M. (2013). "Märchenkorpus Version 1.0" Humboldt-Universität zu Berlin. doi:[10.34644/laudatio-dev-UyRUCnMB7CArCQ9C63ji](https://doi.org/10.34644/laudatio-dev-UyRUCnMB7CArCQ9C63ji).
