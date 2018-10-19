# NDOV Loket PPV/VI voorbeeld XML bestanden

Voorbeeld XML bestanden van verstoringsinformatie, ontvangen via het Infoplus koppelvlak van NDOV Loket. 

## Wat is Infoplus?

Infoplus is het reisinformatiesysteem van de NS, dat gekoppeld is aan 
NDOV Loket via PPV.

## Wat is PPV?

>De verstoringsberichten worden ook beschikbaar gesteld aan 
NS reisinformatiekanalen (zoals internet, reisplanner
xtra app, de reisinformatie in de trein) én aan de NDOV loketten. 
Dit wordt gedaan door het **PPV** (Publicatie
Platform Vervoerders). PPV zorgt ervoor dat informatie over verstoringen 
op alle kanalen altijd consistent en actueel
is, zodat reizigers en personeel overal over dezelfde informatie beschikken.

(bron: NDOV Loket documentatie)

Naast verstoringsinformatie verstuurt dit systeem veel meer data, 
zoals actuele vertrekstaten op stations en realtime positie van treinen.

## Waar komen voorbeelden vandaan

Voorbeelden zijn een sample van echte meldingen die zijn ontvangen via [ZeroMQ queue van NDOV Loket](http://data.ndovloket.nl/REALTIME.TXT).

## Bestandsnaam formaat

```
{type}-{meldingNummer}-{date}.xml
```

- `type`: "PIL" (Patroon Informatie Landerlijk: gestructureerde berichten over verstoringen) of "VTBL" (Vrije Tekst Bericht Landelijk: vrije tekst berichten).
- `meldingsnummer`: Uniek nummer van de melding
- `date`: Datum verstuurd `yymmdd`.

## Licentie

Gegevens worden door NDOV Loket aangeboden onder [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
