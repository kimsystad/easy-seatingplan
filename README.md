# Easy Seatingplan

Nettlesarapp for sceneoppsett til brassband, med norsk (nynorsk) og engelsk grensesnitt. Opne `index.html` direkte i ein nettlesar. Ingen installasjon, byggesteg eller nettilkopling er nødvendig.

## Funksjonar

- Brei scene med standard brassbandoppsett i hestesko eller tom scene.
- Enkel og dobbel stol, notestativ, dirigent, fritekst og stikkebord.
- Slagverksymbol for marimba, vibrafon, xylofon, klokkespel, pauker, trommesett, stortromme (gran cassa), suspended cymbal, clash cymbals med haldar, tam-tam, bongos, skarptromme, triangel, tamburin og røyrklokker.
- Flytting, duplisering, sletting, angring og storleiksjustering av slagverk.
- Stolar, notestativ og utvalde slagverksinstrument vender automatisk mot dirigenten. Instrumentnamna held seg vassrette over objektet.
- Søk etter instrument og utstyr på både norsk og engelsk.
- Teljing av stolar, notestativ, slagverkselement og stikkebord. Stikkebord er òg inkluderte i totalen for slagverkselement.
- Kommadelt slagverksliste som følgjer plasseringane, frå venstre mot høgre sett frå slagverket mot publikum.
- Korpsnamn, konsertopplysningar, riggemerknader og valfri kontaktperson med e-post og telefon.
- Eksport til liggande A4 som PDF og sjølvstendig HTML, med ikonforklaring, slagverksliste, teljing og kontaktinformasjon.
- Automatisk lokal lagring og nedlasting/opning av redigerbare prosjekt som JSON.

## Bruk

1. Vel språk øvst i appen. Språkvalet blir hugsa i nettlesaren og brukt i eksporten.
2. Vel standardoppsettet, eller start med tom scene.
3. Søk etter instrument eller utstyr, vel eit objekt og trykk **Legg til**.
4. Dra elementa på plass. Vel eit element for å endre namn, stoltype, rotasjon, duplisere eller slette. Dra i det grøne hjørnehandtaket for å endre storleiken på slagverk.
5. Fyll inn konsert- og kontaktopplysningar og eksporter til PDF eller HTML.

Piltastane flyttar valt element. Hald Shift for større steg. Rotasjon blir styrt automatisk når objektet følgjer ein dirigent.

**Standard brassband i hestesko** erstattar det opne oppsettet. Lagre prosjektet først dersom du vil ta vare på plasseringane.

## Lagring og eksport

Oppsettet blir lagra automatisk i den aktuelle nettlesaren. Bruk **Lagre prosjekt** for ei JSON-fil som kan opnast og redigerast vidare med **Opne prosjekt**, også på ei anna maskin. Eldre prosjekt utan kontaktfelt kan framleis opnast.

Eksportert HTML er eit sceneoppsett for vising og utskrift, og kan opnast utan nett. PDF-eksporten bruker liggande A4. PDF tek med dei fire første linjene av riggemerknadene; bruk HTML når all merknadsteksten skal vere med.

## Lokal test

Opne `index.html` direkte, eller start ein lokal server frå prosjektmappa:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Opne deretter [den lokale appen](http://127.0.0.1:8000/).

## Personvern og drift

Appen brukar berre lokal lagring i nettlesaren og har ingen eksterne avhengigheiter. Han sender ikkje sceneoppsett eller kontaktinformasjon til ein server. Kontaktinformasjon du fyller inn, blir med i prosjektfilene og eksportane du deler. Sceneplanen er ikkje målsett.

For GitHub Pages kan `index.html` publiserast frå rota av repositoryet. Ingen serverkode eller konfigurasjon er nødvendig.
