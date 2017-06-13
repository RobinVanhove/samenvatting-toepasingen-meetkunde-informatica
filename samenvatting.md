---
title: Samenvatting Toepassing van de Meetkunde in de Informatica
author: Robin Vanhove
date: Juni 2017
toc: true
numbersections: true
geometry: margin=2cm
header-includes:
    \usepackage[dutch]{babel}
    \usepackage{amsfonts}
---

\part{Computergesteund Ontwerp van Curven en Oppervlakken}

# Inleiding
## Situering en Doel
Dit deel gaat over het voorstellen, ontwerpen en analyseren van complexe meetkundige objecten.
Dit wordt in het Engels __Computer Aided Geometric Design__ genoemd. Er zijn twee manieren om een object te beschrijven:

1. Met behulp van een groot aantal punten, dit is niet nauwkeurig en moeilijk om met te werken.
2. Met een wiskundig model waarin enkele parameters gekozen worden die het object beschrijven.

We zullen dan ook de tweede manier toepassen en een wiskundige beschrijving van curven en oppervlakken zoeken. Vervolgens zullen we algoritmen opstellen om ermee te rekenen.

## Basisbegrippen
### Punten en Vectoren
__Punten__ zijn elementen in een __affiene ruimte__ $\mathbb{E}^2$ of $\mathbb{E}^3$ (2, 3 dimensies). In dergelijke ruime bekleed een punt geen belangrijkere plaats dan een ander punt, er is dus geen oorsprong of assenstelsel. 

__Vectoren__ zijn elementen van een vectorruimte $\mathbb{R}^2$ of $\mathbb{R}^3$. Ze hebben een richting, een zin en een lengte.

Om berekeningen met punten te maken moeten we toch een assenstel kiezen, waardoor we punten behandelen als vectoren.

$$ \vec{p} = 
\begin{bmatrix} 
    x\\
    y\\
\end{bmatrix}
= [x, y]^T
~\text{of}~
\vec{p} = 
\begin{bmatrix} 
    x\\
    y\\
    z\\
\end{bmatrix}
= [x, y, z]^T
$$

Een __affiene combinatie__ ofwel _barycentrische_ combinatie is een gewogen combinatie (som) van punten waarbij de gewichten sommeren tot 1.

$$ \vec{x} = \sum ^m_{i=1} \alpha_i \vec{p_i} ~\text{ met }~  \alpha_1 + \alpha_2 + ... + \alpha_m$$

### Curven en Oppervlakken
Een __curve__ verschilt van een klassieke functie door zijn mogelijke meerwaardigheid. Dus een curve kan meerdere y-waarden hebben voor 1 x-waarde. Een curve kan voorgesteld worden in functie van een variabele u die fungeert als parameter.

$$\vec{x(u)} = 
\begin{bmatrix} 
    f_1(u)\\
    f_2(u)\\
\end{bmatrix}
~\text{ met }~ u \in [a, b]
$$

Een oppervlak wordt gegeven door $\vec{x}(\vec{u})$ waar $\vec{u} = [u, v]^T$ het beeld van een rechthoek is.

### Segmentatie en lokale parameters
__Segmentatie__ is het opdelen van een curve of oppervlak in meerdere stukken ook _segmenten_ genoemd. Men kiest een aantal __knooppunten__ die het interval opsplitsen in deelintervallen. Met ieder deelinterval komt er een segment $\vec{x_0}(u)$ overeen. De functie zet de __globale parameter__ $u$ vaak om naar een __lokale parameter__ $t$ die beschreven wordt in functie van $u$. Het segment wordt dan geschreven als $\vec{x_0}(t(u))$.

### Affiene Transformaties
Een transformatie is __affien__ als elke affiene combinatie van een stel punten afgebeeld wordt op diezelfde affiene combinatie van de beelden van die punten. Dus elk punt dat gegeven wordt door
$$ \vec{x} = \sum ^m_{i=1} \alpha_i \vec{p_i} ~\text{ met }~  \alpha_1 + \alpha_2 + ... + \alpha_m$$
wordt afgebeld op het op het put
$$w(\vec{x}) = \sum_{i=1}^m \alpha_iw(\vec{p_i})$$
In andere woorden, affiene combinaties zijn invariant onder affiene transformaties.

Een affiene transformatie kan geschreven worden in de vorm.
$$w(\vec{x}) = A\vec{x}+\vec{v}$$

### Convex Omhullende en Convexe Combinatie
## Interpolerende veeltermcurven

# Bézier-curven
## Definities
## Eigenschappen van Bernstein-veeltermen
## Enkele Eigenschappen van Bézier-curven
## Evaluatie van een Punt op een Bézier-curve
## Afgeleiden van een Bézier-curve
## Graadverhoging
## Opsplitsing van een Bézier-curve
## Samengestelde Bézier-curven
## Ontwerp en Modellering van Complexe Bézier-curven
## Toepassing: lettertypes voor laserprinters
## Besluit

# Splinecurven
# Modellering van Oppervlakken

\part{Algoritmen voor Discrete Meetkundige Problemen}

# Inleiding
# Algoritmen voor Eenvoudige Meetkundige Problemen
# Berekening an de Convex Omhullende
# Het Dichtste Puntenpaar en het Verste Puntenpaar
# Het Vornoi-diagram van een puntenverzameling
# Nabijheidsproblemen
# Berekening van het Vornoi-diagram
