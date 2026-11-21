# Spletna trgovina s pajkicami

Vaja_RPO je skupinski projekt pri predmetu Razvoj programske opreme, v katerem po metodi Scrum razvijamo spletno trgovino z ženskimi pajkicami in športnimi oblačili. Trgovina bo omogočala pregled in filtriranje produktov, košarico, registracijo uporabnikov ter pregled preteklih naročil.

> Ime trgovine: **[dopolni]**. Vrednosti, označene kot *predlog*, so naše odločitve za projekt in jih lahko še spremenimo.

## O trgovini

Trgovina prodaja ženske pajkice in oblačila za šport in vsakdan: dolge, capri, termo in brezšivne pajkice ter hlače za vsak dan. Namenjena je kupkam, ki želijo udobna in kakovostna oblačila po dostopni ceni in jih hitro najti po velikosti, barvi in namenu.

Trgovina ima tudi fizične poslovalnice. Vsaka poslovalnica ima svoj nabor kategorij, kupec pa lahko naročilo prevzame osebno.

## Ponudba

| Kategorija | Opis |
|---|---|
| Dolge pajkice | Visok pas, za šport in vsak dan |
| Capri pajkice | Krajše, do sredine meč, za toplejše dni |
| Termo pajkice | Notranja podloga za hladne dni |
| Brezšivne pajkice | Brez šivov, raztegljiv material |
| Hlače za vsak dan | Elegantnejši kroj za službo in prosti čas |
| Outlet | Znižani izdelki iz prejšnjih kolekcij |

Vsak izdelek ima:

| Lastnost | Primer |
|---|---|
| Naziv | Dolge pajkice z visokim pasom |
| Kategorija | Dolge pajkice |
| Znamka in dobavitelj | [dopolni] |
| Velikosti | XS, S, M, L, XL, XXL |
| Barve | črna, temno modra, rjava, zelena |
| Material | 80 % poliamid, 20 % elastan |
| Cena | 19,90 € (z DDV) |
| Zaloga | na zalogi / zadnji kosi / ni na zalogi |
| Kratek in dolg opis, tehnične podrobnosti | navodila za pranje, debelina materiala |
| Garancija | 2 leti |
| Oznaka | "novo", "akcija" |

## Kako trgovina deluje

1. **Brskanje.** Kupec na domači strani vidi izpostavljene in najbolj prodajane izdelke ali izbere kategorijo v meniju.
2. **Iskanje izdelka.** Seznam izdelkov je razdeljen na strani. Kupec ga uredi po ceni ali nazivu in filtrira po kategoriji, velikosti, barvi, znamki, dobavitelju, razpoložljivosti in ceni.
3. **Stran izdelka.** Kupec izbere velikost in barvo, prebere opis, tehnične podrobnosti in garancijo ter doda izdelek v košarico.
4. **Košarica.** Kupec spremeni količine ali odstrani izdelke. Trgovina sproti izračuna vmesno vsoto, DDV, stroške dostave in skupno ceno.
5. **Oddaja naročila.** Prijavljen kupec ima naslov že izpolnjen. Neregistriran kupec vpiše naslov za dostavo. Kupec izbere način plačila in dostave ter odda naročilo.
6. **Potrditev.** Kupec vidi številko naročila; prijavljen kupec ga najde tudi v pregledu preteklih naročil.

### Cene, dostava in plačilo (predlog)

- Cene so prikazane z DDV (22 %); v košarici je DDV izpisan posebej.
- Dostava: 3,90 €, brezplačna pri naročilu nad 40 €. Osebni prevzem v poslovalnici je brezplačen.
- Načini dostave: Pošta Slovenije, dostavna služba, osebni prevzem v poslovalnici.
- Načini plačila: po povzetju, plačilna kartica, PayPal. Izbira je samo vizualna; pravega plačila ne izvajamo.

### Statusi naročila

Prejeto → V obdelavi → Poslano → Dostavljeno, ali Preklicano.

## Strani trgovine

| Stran | Kaj prikazuje |
|---|---|
| Domača stran | Izpostavljeni izdelki, najbolj prodajani po kategorijah, prednosti nakupa (brezplačna dostava, varen nakup, garancija), mnenja kupcev, izbira jezika |
| Kategorija / seznam izdelkov | Izdelki z imenom, ceno, razpoložljivostjo, kratkim opisom in gumbom "Dodaj v košarico"; paginacija, urejanje, filtri |
| Stran izdelka | Izbira velikosti in barve, daljši opis, tehnične podrobnosti, garancija, povezava do uradne strani, mnenja (izbirno) |
| Košarica | Izdelki, količine, cene, DDV, dostava, skupaj, izbira plačila in dostave, naslov za neregistrirane |
| Registracija in prijava | Obrazca za nov račun in prijavo, pozabljeno geslo |
| Profil | Ime, priimek, e-pošta, naslov za dostavo, telefon; urejanje podatkov |
| Moja naročila | Številka, status, izdelki, količine, datum in skupna cena vsakega naročila |
| Poslovalnice (izbirno) | Naslov, delovni čas, kontakt, vodja, obvestila in zemljevid |

## Uporabniški račun

- **Registracija:** ime, priimek, e-pošta, geslo, naslov za dostavo, telefon.
- **Prijava:** e-pošta in geslo.
- **Pozabljeno geslo:** kupec vpiše e-pošto in prejme povezavo za nastavitev novega gesla.
- **Profil:** kupec lahko kadarkoli uredi svoje podatke.
- Pretekla naročila vidijo samo registrirani uporabniki.

## Jeziki

Na domači strani je gumb za izbiro jezika z zastavo in imenom jezika: slovenščina in angleščina. Ob menjavi se spremeni besedilo na vseh straneh.

## Podatkovni model

| Tabela | Glavni podatki |
|---|---|
| uporabniki | ime, priimek, e-pošta, geslo (zgoščeno), naslov, telefon |
| kategorije | naziv, opis |
| izdelki | naziv, kategorija, znamka, dobavitelj, cena, opisi, garancija, material |
| različice | izdelek, velikost, barva, zaloga |
| poslovalnice | naziv, naslov, delovni čas, kontakt, vodja |
| poslovalnice_kategorije | katere kategorije ima posamezna poslovalnica |
| naročila | številka, uporabnik ali podatki gosta, datum, status, način plačila in dostave, skupna cena |
| postavke_naročila | naročilo, različica izdelka, količina, cena ob nakupu |
| mnenja (izbirno) | izdelek, uporabnik, ocena 1 do 5, besedilo |

## Dostopnost in oblikovanje (izbirno)

- Alternativni opisi slik, oznake za bralnike zaslona, delo s tipkovnico in gumb "Skoči na vsebino".
- Kontrast vsaj 4,5:1, prilagoditev za različne zaslone, preverjanje z orodjem WAVE.
- Izbira barvne teme (privzeta in monokromatske teme), shranjena v localStorage.
- Prehodi med stranmi, animacije ob prehodu z miško in namigi (tooltip).

## Tehnologije in zagon

Tehnologije: **[dopolni: jezik, ogrodje, podatkovna baza]**

```bash
git clone git@github.com:dukoski780/Vaja_RPO.git
cd Vaja_RPO
# [dopolni: namestitev odvisnosti, nastavitev baze, ukaz za zagon]
```

## Skupina

| Član | GitHub | Vloga |
|---|---|---|
| Martin Dukoski | [dukoski780](https://github.com/dukoski780) | [dopolni] |
| Jure Kos | [jurethekos](https://github.com/jurethekos) | [dopolni] |
| Gregor Mlakar | [GregorMlakar](https://github.com/GregorMlakar) | [dopolni] |

## Razvoj

- **Git:** `dev` je razvojna veja, `master` vsebuje delujočo različico. Pred združitvijo naredimo `git pull`, razrešimo konflikte in preverimo, da trgovina deluje.
- **Scrum:** nabor zgodb, cikli in burndown so v [Jiri](https://rpo-spletna-trgovina.atlassian.net) (prostor SCRUM). Na koncu vsakega cikla imamo revizijo in retrospektivo. Metrika: hitrost (velocity).

| Cikel | Cilj | Načrtovane točke | Dokončane točke |
|---|---|---|---|
| 1 | Postavitev projekta, baza, prijava in registracija | | |
| 2 | Seznam izdelkov, stran izdelka, košarica | | |
| 3 | Pretekla naročila, izbira jezika, dokumentacija, izbirne naloge | | |
