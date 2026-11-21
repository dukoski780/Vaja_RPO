# RPO – MGJ: spletna trgovina s pajkicami in športnimi oblačili

RPO – MGJ je skupinski projekt pri predmetu Razvoj programske opreme, v katerem po metodi Scrum razvijamo spletno trgovino z ženskimi pajkicami in športnimi oblačili. Trgovina bo omogočala pregled in filtriranje izdelkov, nakupovanje prek košarice, registracijo uporabnikov ter pregled preteklih naročil.

## O trgovini

Trgovina prodaja ženske pajkice ter udobna oblačila za šport in vsakdan. Ponuja različne modele, od klasičnih in krajših pajkic do toplih zimskih in brezšivnih modelov.

Namenjena je kupkam, ki iščejo udobna, kakovostna in cenovno dostopna oblačila. Izdelke lahko preprosto poiščejo glede na velikost, barvo, ceno in namen uporabe.

Trgovina ima več poslovalnic, pri čemer vsaka ponuja svoj izbor kategorij izdelkov.

## Ponudba

| Kategorija | Opis |
|---|---|
| Dolge pajkice | Klasične dolge pajkice, primerne za šport in vsakodnevno nošenje |
| 3/4 pajkice | Krajše pajkice, ki segajo pod kolena oziroma do sredine meč, primerne za toplejše dni |
| Tople pajkice | Pajkice s toplo notranjo podlogo za hladnejše dni |
| Brezšivne pajkice | Raztegljive pajkice z minimalnim številom šivov za večje udobje |
| Hlače za vsak dan | Udobne hlače za službo, prosti čas in vsakodnevne aktivnosti |
| Outlet | Znižani izdelki iz prejšnjih kolekcij |

Vsak izdelek ima:

| Lastnost | Primer |
|---|---|
| Naziv | Dolge pajkice z visokim pasom |
| Kategorija | Dolge pajkice |
| Znamka in dobavitelj | ime znamke in dobavitelja |
| Velikosti | XS, S, M, L, XL, XXL |
| Barve | črna, temno modra, rjava, zelena |
| Material | 80 % poliamid, 20 % elastan |
| Cena | 19,90 € (z DDV) |
| Zaloga | na zalogi / zadnji kosi / ni na zalogi |
| Kratek in dolg opis, tehnične podrobnosti | navodila za pranje, debelina materiala |
| Garancija | 2 leti |
| Povezava | uradna stran izdelka |

## Kako trgovina deluje

1. **Brskanje.** Kupec na domači strani vidi izpostavljene izdelke ali izbere kategorijo v meniju.
2. **Iskanje izdelka.** Seznam izdelkov je razdeljen na strani. Kupec ga uredi po ceni ali nazivu in filtrira po kategoriji, velikosti, barvi, znamki, dobavitelju, razpoložljivosti in ceni.
3. **Stran izdelka.** Kupec izbere velikost in barvo, prebere opis, tehnične podrobnosti in garancijo ter doda izdelek v košarico.
4. **Košarica.** Kupec spremeni količine ali odstrani izdelke. Trgovina sproti izračuna vmesno vsoto, davek, stroške dostave in skupno ceno.
5. **Oddaja naročila.** Prijavljen kupec ima naslov že izpolnjen. Neregistriran kupec vpiše naslov za dostavo. Kupec izbere način plačila in dostave (samo vizualno) ter odda naročilo.
6. **Potrditev.** Kupec vidi številko naročila; prijavljen kupec ga najde tudi v pregledu preteklih naročil.

### Statusi naročila

Prejeto → V obdelavi → Poslano → Dostavljeno, ali Preklicano.

## Strani trgovine

| Stran | Kaj prikazuje |
|---|---|
| Domača stran | Izpostavljeni izdelki, kategorije, izbira jezika |
| Kategorija / seznam izdelkov | Izdelki z imenom, ceno, razpoložljivostjo, kratkim opisom in gumbom "Dodaj v košarico"; paginacija, urejanje, filtri |
| Stran izdelka | Izbira velikosti in barve, daljši opis, tehnične podrobnosti, garancija, povezava do uradne strani, gumb "Dodaj v košarico" |
| Košarica | Izdelki, količine, cene, davek, dostava, skupaj, izbira plačila in dostave, naslov za neregistrirane |
| Registracija in prijava | Obrazca za nov račun in prijavo, pozabljeno geslo |
| Profil | Ime, priimek, e-pošta, naslov za dostavo, telefon; urejanje podatkov |
| Moja naročila | Številka, status, izdelki, količine, datum in skupna cena vsakega naročila |

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
| poslovalnice | naziv, naslov |
| poslovalnice_kategorije | katere kategorije ima posamezna poslovalnica |
| naročila | številka, uporabnik ali podatki gosta, datum, status, način plačila in dostave, skupna cena |
| postavke_naročila | naročilo, različica izdelka, količina, cena ob nakupu |

## Skupina

| Član | GitHub | Vloga |
|---|---|---|
| Martin Dukoski | [dukoski780](https://github.com/dukoski780) | Scrum mojster, razvijalec |
| Jure Kos | [jurethekos](https://github.com/jurethekos) | Razvijalec |
| Gregor Mlakar | [GregorMlakar](https://github.com/GregorMlakar) | Razvijalec |

Vlogo lastnika izdelka si delimo vsi trije.
