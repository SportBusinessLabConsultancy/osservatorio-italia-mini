# Osservatorio Italia — Mappa (versione pubblica)

Versione ridotta e pubblica del geoportale **Osservatorio Italia**, sviluppato durante lo stage in
Sport Lab. Mostra su una mappa interattiva dell'Italia alcuni livelli tematici a punti/dati leggeri
(edifici scolastici, strutture sportive, luoghi turistici, mappa culturale, stazioni, bus, aree
pubbliche, biblioteche, parchi).

## 🗺️ Apri la mappa

**[Apri la mappa live](https://SportBusinessLabConsultancy.github.io/osservatorio-italia-mini/)**

*(link da verificare/correggere con lo username GitHub esatto una volta attivato GitHub Pages)*

## Cos'è questa versione

Questa è una versione **ridotta** pensata per essere pubblicata gratuitamente su GitHub Pages, con
un link consultabile da chiunque. Include solo i livelli di dati più leggeri (sotto i 100 MB per
file, il limite di GitHub).

**Non sono inclusi in questa versione** (troppo pesanti per un hosting gratuito):
- Isocrone di accessibilità (tempo di percorrenza per raggiungere scuole, parchi, ecc.)
- Aree verdi (poligoni, ~355 MB)
- Rete idrica (poligoni/linee, 126-355 MB)

La versione **completa**, con tutti i dati (inclusi isocrone, aree verdi, rete idrica e dati grezzi),
è disponibile sul server interno dell'azienda (My Cloud Home).

## Struttura del progetto

```
osservatorio-italia-mini/
├── index.html                          # pagina della mappa
├── style.css                           # stile
└── data/
    ├── edifici_scolastici.geojson
    ├── aree_pubbliche.geojson
    ├── biblioteche.geojson
    ├── parchi.geojson
    ├── stazioni.geojson
    ├── mappa_culturale.geojson
    ├── luoghi_turistici.geojson
    ├── bus.geojson
    └── strutture_sportive_regioni/     # strutture sportive, divise per regione
        ├── abruzzo.geojson
        ├── ...
        └── veneto.geojson
```

## Come vedere la mappa in locale (senza GitHub Pages)

Dalla cartella principale del progetto (`osservatorio-italia-mini/`), lancia:

```
python -m http.server
```

Poi apri nel browser:

```
http://localhost:8000/index.html
```

## Autore

Carlo Pegoraro — stage Sport Lab, 2026.
