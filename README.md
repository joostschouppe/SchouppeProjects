# Spatial Join in SPSS

Je kan een spatial join van punten in polygonen doen binnen SPSS.
Dat betekent: als je X-Y coördinaten in je bestand hebt zitten, dan kun je deze verrijken met informatie over polygonen. Bijvoorbeeld kan je op die manier aan een Antwerpse adrescoördinaat een statistische sector toekennen.
Dit kan je natuurlijk omzeilen door over ArcGIS te gaan, maar dat kan nogal omslachtig zijn.
Deze methode doet op een trager PC zo’n 100.000 records per minuut.

Je vindt in deze map een voorbeeld waarbij een bestand wordt verrijkt met sector_gesplitst. In het script wordt alles stap voor stap uitgelegd.

Dit voorbeeld zal enkel werken indien je Python versie over een aantal libraries beschikt die nodig zijn. 
 
Dit script werkt als je Anaconda installeert, en de “Python location” daarnaar laat verwijzen. Ga daarvoor naar Edit>Options>File Locations>Python (2.7) Location.
Zoals je ziet vraagt SPSS naar een versie 2.7 van Python. Kies dus voor een Anaconda versie met Python 2.7 (https://www.continuum.io/downloads). Bij installeren heb je mogelijk admin rechten nodig. Als je “Installeren alleen voor jou”  kiest, dan moet je in SPSS verwijzen naar een locatie als C:\Users\[jouw unieke naam]\AppData\Local\Continuum\Anaconda2.

Het kan geen kwaad als je meerdere Python versies op je PC hebt, zoals die van SPSS, die van ArcGIS,... 

Eens geïnstalleerd, voer volgende commando uit in de Anaconda prompt (een van de programma's binnen het Anaconda pakket):

```conda install -c ioos shapely rtree pyshp```

Je vindt in deze repository een voorbeeldscript.

## Bronnen

Het script is van https://andrewpwheeler.wordpress.com/2016/12/09/spatial-join-points-to-polygons-using-python-and-spss/ , 
gebaseerd op http://rexdouglass.com/fast-spatial-joins-in-python-with-a-spatial-index/ en verbeterd met hulp van [@warrieka](https://github.com/warrieka)
