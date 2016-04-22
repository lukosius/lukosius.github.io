---
layout: post
title:  "[LT] OJS 2.4.8 CrossRef konfigūravimo užrašai"
---

## Pagrindinės sąvokos

[Digital Object Identifier][link-doi] (**DOI**) - globaliai unikalus identifikarius skirtas skaitmeniniams objektams. 
OJS sistemoje tai būtų žurnalai, žurnalo numeriai, straipsniai ir papildomi failai.

[Crossref][link-crossref] - oficiali DOI raktų išdavimo agentūra.

## Privaloma informacija

CrossRef įskiepis reikalauja pateikti šiuos duomenis žurnalo konfigūravimo pirmajame žingsnyje:

- Žurnalo pavadinimas
- Žurnalo inicialai
- Žurnalo santrumpa
- Žurnalo ISSN
- Pagrindinis kontaktas (vardas ir el. paštas)
- Techninės pagalbos kontaktas (vardas ir el. paštas)
- Leidėjas (institucija ir URL)

## DOI įskiepis

_Sistemos įskiepiai -> Viešojo identifikatoriaus įskiepiai -> DOI įskiepis._

Pirmiausia įskiepį įgalinti ir tuomet atverti jo nustatymus, kuriuose reikia nustatyti,
kokiam žurnalo turiniui bus priskiriami DOI. Čia būtina pažymėti **straipsnius** ir **papildomus failus**.

Toliau reikia įvesti **DOI prefix**, kurį suteikė Crossref.

Papildomai galima sukonfigūruoti ir **DOI suffix**, bet OJS rekomenduojama naudoti numatytuosius parametrus.

## CrossRef įskiepis

_Importavimas/Eksportavimas -> CrossRef eksportavimo/registracijos įskiepis_

Atvėrus įskiepio nustatymus bus rodoma, kurie bendrieji sistemos reikalavimai yra patenkinti. Čia galimos klaidos:

- Neįgalintas ar nesukonfigūruotas DOI įskiepis
- Nesukonfigūruotas Crossref įskiepis
- Nenurodyta privaloma informacija skirta Crossref įskiepiui

Depozitoriaus vardas ir el. pašto adresas bus paimti iš pagrindinio kontakto, tačiau šią informaciją galima keisti.

Jei pateikiami CrossRef prisijungimo duomenys (vartotojo vardas ir slaptažodis) bus galima aktyvuoti
automatinį DOI registravimą. OJS straipsnių DOI pateiks automatiškai į CrossRef, kai straipsniai yra išleidžiami.
Šis procesas gali šiek tiek užtrukti.

Visus neregistruotus DOI galima peržiūrėti neregistruotų straipsnių sąraše.

## Nesklandumai

Pradinius nesklandumus aptinka CrossRef eksportavimo/registravimo įskiepis, kuris praneša apie konfigūracijos klaidas bandant
pateikti DOI. Rodomos klaidos yra savaime suprantomos, todėl jas ištaisyti paprastai užtenka patikrinti, kuris konfigūracijos
žingsnis buvo praleistas, patikrinti CrossReg prisijungimo duomenis. Papildomai gali rodyti klaidą jei paslauga dėl kurių nors priežasčių yra neprieinama.

Dažniausiai gali pasitaikyti XML klaidos, kurias galima patikrinti CrossRef svetainėje su [metaduomenų kokybės patikros][link-validation] įrankiu.

## Nuorodos

1. [CrossRef dokumentacija](https://pkp.sfu.ca/wiki/index.php?title=CrossRef)
2. [DOI įskiepio dokumentacija](https://pkp.sfu.ca/wiki/index.php?title=DOIPluginsDocumentation)

[link-doi]: http://dx.doi.org
[link-crossref]: http://www.crossref.org
[link-validation]: http://www.crossref.org/02publishers/parser.html
