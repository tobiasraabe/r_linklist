
R Linkliste
===========

[Table of contents](https://tableofcontents.herokuapp.com)
- [Installation](#installation)
  - [R Distribution](#r-distribution)
  - [IDE (Integrated Development Environment)](#ide-integrated-development-environment)
    - [Jupyter](#jupyter)
      - [Installation](#installation)
    - [RStudio](#rstudio)
- [Packages](#packages)
  - [Tidyverse](#tidyverse)
  - [Simple Features](#simple-features)
- [Hilfe](#hilfe)

# Installation

## R Distribution

Microsoft bietet eine R-Distribution an, [Microsoft R Open]
(https://mran.microsoft.com/open/), die mit den meistgenutzten Packages
kompatibel ist.


## IDE (Integrated Development Environment)

Eine IDE ist eine Entwicklungsumgebung in der programmiert wird. Für die
Datenarbeit ist eine guter Mix aus Visualisierung und Texten nötig.

Hier gibt es zwei Möglichkeiten von denen mindestens eine genutzt werden
sollte, aber auch die Kombination aus beiden kann nützlich sein.

### Jupyter

[Jupyter](http://jupyter.org/) ist eine Python-basierte IDE, die mehrere
Programmiersprachen unterstützt. Hauptmerkmal sind die Notebooks genannten
Programmierumgebungen, in denen fließend Textzellen (Markdown-Format) und
Codezellen verbunden werden können. Ebenso lassen sich Grafiken leicht
einbetten. Für einen Bericht lässt sich das Notebook leicht in eine PDF
konvertieren.

#### Installation

1. Installiere [Anaconda für Python 3.x](https://www.continuum.io/downloads)
2. Installiere [Microsoft R Open](https://mran.microsoft.com/open/)
3. Installiere [IRkernel](https://github.com/IRkernel/IRkernel), um Jupyter mit
   R zu nutzen
   - Es kann ein Fehler auftreten, dass ``stringr`` nicht installiert ist.
   ``install.packages(stringr)`` ausführen und Schritte wiederholen.
   - Beim Schritt, in dem der Kernel registriert wird, den String an die
   passende Versionsnummer von R anpassen

### RStudio

[RStudio](https://www.rstudio.com/) ist eine weitere IDE für R. Die Funktionen
decken sich mit denen von Jupyter, aber die Umsetzung scheint ein wenig
schwieriger zu sein als mit Jupyter.


# Packages

Das Problem mit Packages unter R ist, dass es soviele mit gleichen oder
überlappenden Funktionen gibt. Dazu passiert es oft, dass man auf Vorläufer von
neueren Packages verwiesen wird oder stößt. Gute Möglichkeiten, um den Dschungel
zu durchkämmen bieten:
- https://rseek.org/: eine R-Suchmaschine für Packages, Tutorials, etc.
- https://mran.microsoft.com/packages: der Package Manager von MRO biete zu
  jedem Package hilfreiche Links, etc.

## Tidyverse

Das [Tidyverse](http://tidyverse.org/) ist eine Ansammlung von Packages und
sollte die erste Anlaufstelle bei der Suche nach einer Funktion sein. Hier ist
eine kurze Liste der Packages mit Funktionen:

- **Haven**: Einlesen und Schreiben von Datensätzen von Statistikprogrammen wie
  Stata, SAS, SPSS
- **readr**: Einlesen und Schreiben von Datensätzen im Format .csv, .tsv, .fwf
- **dplyr**: Funktionen zur Datenmanipulation, gruppieren, selektieren,
  filtern, etc.
- **magrittr**: Ermöglicht das Schreiben von Pipelines in R, um lesbareren Code
  zu schrieben
- **stringr**: Funktionen zur Manipulation von Strings
- **tidyr**: Funktionen, um seine Daten zu säubern
- **ggplot2**: Erstellen von Grafiken
- **packrat**: Dependency management für R-Projekte
- **lintr**: Beim Linting wird der Code mit einem Style Guide verglichen, um
  die Lesbarkeit des Codes zu erhöhen

## Simple Features

[Simple Features](https://github.com/r-spatial/sf) scheint das neueste Package
für die Arbeit mit geographischen Daten zu sein. Die Dokumentation ist eher
schlecht als recht, aber es gibt ein paar Tutorials und Vignettes als Links auf
der Seite.


# Hilfe

- https://stackoverflow.com/ und alle anderen Stack-websites
- Dokumentation der Packages
