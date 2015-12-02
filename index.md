---
layout: ribbon

style: |
    .slide:after {
        display: none;
    }

    #Cover {
        background: url("pictures/cover.jpg");
        background-size: cover;
        color:#FFF;
    }
    #Cover h2 {
        margin:30px 0 0;
        color:#FFF;
        text-align:center;
        font-size:70px;
        }
    #Cover h3 {
        margin:10px 0 0;
        text-align:center;
        font-style:italic;
        font-size:40px;
        }
    #Cover p {
        margin:10px 0 0;
        text-align:center;
        color:#FFF;
        font-style:italic;
        font-size:20px;
        }
        #Cover p a {
            color:#FFF;
            }
---

# Une (brève) histoire du temps {#Cover}

*Historique des standards du temps, par [Julien Tanguy](http://twitter.com/jutanguy)*

<!-- cover image from https://en.wikipedia.org/wiki/Black_hole  -->

## **tempus fugit**

## Sur les rives de Babylone

- 1 jour = 12 danna (2 heures)
- 1 danna = 30 ush (4 minutes)
- 1 ush = 60 nindan (4 secondes)

{:.note}
La minute vient du latin _minuta_, partie menue de la division (de l'heure ou du degré)

## Calendrier babylonien

- Calendrier lunaire, puis luni-solaire
- 1 an = 12 mois
- 1 mois intercalaire supplémentaire les années 3, 6, 8, 11, 14, 17 et 19 (Cycle métonique)

{:.note}
Le mot seconde vient de "seconde subdivision par 60 d'une heure"


## Du côté du phare d'Alexandrie

- 1 an = 12 mois de 30 jours + 5 jours
- La nuit est divisée en 12h
    - Le ciel était divisé en 36 décans
    - Seulement 12 étaient observables en une nuit
- Le jour a été divisé en 12h par symmétrie de la nuit

{:.note}
Nos 24 heures sont égyptiennes

## Calendriers

- Lunaire: musulman
- Luni-solaire: chinois, hébraïque, tibétain
- Solaire: julien, grégorien

{:.note}
Le calendrier grégorien, instauré le 15 octobre 1582, ne remplace pas les dates antérieures


## Jour julien

- Créé par Joseph Juste Scaliger, en l'honneur de Jules César Scaliger
- Compté en nombres de jours + fraction de jour par rapport à une origine
- Origine du jour julien: 1 janvier -4712 à midi
    - Avant la totalité de l'histoire connue
    - Lundi 1er janvier
    - Année bissextile
    - Début de cycle métonique
    - Début de cycle d'indiction romaine

{:.note}
Variantes du jour julien en décalant l'origine: MJD, TJD


## TODO

- Mesure de la seconde
- Time zones
- UT0, UT1, TAI, UTC, Leap seconds

## Conseils

- Stockage UTC + visu localisée
- Sérialisation: ISO 8601
- Ne réinventez pas l'horloge
