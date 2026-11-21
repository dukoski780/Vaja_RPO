# Vaja_RPO – Spletna trgovina

Vaja_RPO je skupinski projekt pri predmetu Razvoj programske opreme, v katerem po metodi Scrum razvijamo spletno trgovino z ženskimi pajkicami in športnimi oblačili. Trgovina bo omogočala pregled in filtriranje produktov, košarico, registracijo uporabnikov ter pregled preteklih naročil.

## Ponudba

- Kategorije: dolge pajkice, capri pajkice, termo pajkice, brezšivne pajkice, hlače za vsak dan, outlet
- Lastnosti izdelka: velikost (XS do XXL), barva, material, kolekcija, cena, zaloga in oznaka "novo"
- Domača stran: izpostavljeni izdelki, najbolj prodajani izdelki po kategorijah, mnenja kupcev, prednosti nakupa (brezplačna dostava, varen nakup, garancija)
- Slog: čista, svetla stran z velikimi fotografijami izdelkov in kratkimi, prijaznimi besedili

## Skupina

| Član | GitHub | Vloga |
|---|---|---|
| Martin Dukoski | [dukoski780](https://github.com/dukoski780) | [dopolni] |
| Jure Kos | [jurethekos](https://github.com/jurethekos) | [dopolni] |
| Gregor Mlakar | [GregorMlakar](https://github.com/GregorMlakar) | [dopolni] |

## Funkcionalnosti

Osnovni nivo (obvezno):

- [ ] Podatkovna baza: uporabniki, produkti in kategorije, poslovalnice, naročila
- [ ] Seznam produktov: paginacija, urejanje po ceni in nazivu, filtri (kategorija, velikost, barva, znamka, dobavitelj, razpoložljivost, cena), stran o produktu
- [ ] Košarica: količina, cena, davek, dostava, izbira plačila in dostave, oddaja naročila
- [ ] Registracija, prijava, urejanje profila in pozabljeno geslo
- [ ] Pregled preteklih naročil za registrirane uporabnike
- [ ] Izbira jezika na vseh straneh

Napredni nivo (izbirno):

- [ ] Seznam poslovalnic z zemljevidom
- [ ] Ocene, mnenja in slike produktov
- [ ] Napredno oblikovanje in dostopnost (WAVE, izbira barvne teme)

## Tehnologije

[dopolni: jezik, ogrodje, podatkovna baza]

## Namestitev in zagon

```bash
git clone git@github.com:dukoski780/Vaja_RPO.git
cd Vaja_RPO
# [dopolni: namestitev odvisnosti, nastavitev baze, ukaz za zagon]
```

## Delo z Gitom

- `master` vsebuje delujočo, oddano različico.
- `dev` je razvojna veja; nove funkcionalnosti razvijamo na njej ali na vejah iz nje.
- Pred združitvijo v `master` naredimo `git pull`, razrešimo konflikte in preverimo, da projekt deluje.

## Vodenje projekta (Scrum)

- Nabor zgodb, cikli in burndown: [Jira](https://rpo-spletna-trgovina.atlassian.net) (prostor SCRUM)
- Trije cikli; na koncu vsakega cikla revizija in retrospektiva
- Metrika agilnih metod: hitrost (velocity) in burndown po ciklih

| Cikel | Cilj | Načrtovane točke | Dokončane točke |
|---|---|---|---|
| 1 | Postavitev projekta, baza, prijava in registracija | | |
| 2 | Seznam produktov, stran produkta, košarica | | |
| 3 | Pretekla naročila, izbira jezika, dokumentacija, izbirne naloge | | |
