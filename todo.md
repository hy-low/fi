---
title: TODO
permalink: /todo
hide: true
---

# TODO

## Yleistä

- Paluuarvo vai palautusarvo?
- Virtuaalinen muisti vs. fyysinen muisti, tuo esille usein
- Rakenne `enum`
- Mitkä parametrit käännöksessä? (`-Wall`, `-Wextra`, `-O2`, `-std=c99`, `-pedantic`)
- Varmista että kaikkialla `void` jos funktiolla ei ole parametreja
- Mikä on `main`-funktion palautusarvo ja miksi on tai ei ole `return 0`
- Mikä on POSIX?
- Syntaksi `\` merkeissä ja merkkijonoissa
- Lukujen kantajärjestelmät paremmin?
- Liukuluvut kattavammin?
  - Tieteellinen notaatio
  - Mitä voidaan esittää tarkasti liukuluvuilla
- Standardikirjaston funktioihin linkit referenssiin?
- Muutenkin tietoa C-referensseistä netissä? Entä C-kirjat?
- Funktio `exit` lopettaa ohjelman -> esittele virheenkäsittelyssä?
- Bittisyys historiassa? 8, 16, 32, 64?
- float muuttuu doubleksi vaihtuvassa parametrilistassa, entä muut?
- Samaa tunnusta voidaan käyttää monessa yhteydessä?
- Turvallisuus ei ollut samassa roolissa ennen
- Virheenkäsittely ohjelmissa??
- Muistihierarkiat (rekisterit, välimuistit)
- `getchar`, `putchar`, `gets`, `puts`
- `int` oletustyyppi, jäänne `unsigned` = `unsigned int`
- `int*` tarkoittaa sekä osoite yhteen lukuun että taulukkoon
- Mitä `#include` oikeastaan tekee?
- Avainsanat `register` ja `volatile`
- Esittele mielekäs osa tiedostosta `stdio.h`?
- `return x - y` ei toimi oikein järjestämisessä?

## Luku 1

- Lohko vs. lause ehdoissa ja silmukoissa
- Operaattoreiden presedenssi
- Lausekkeen osien suoritusjärjestys (and, or)
- Suoritusjärjestys ei aina selvä
- Duff's device? tai muuten switch tarkemmin
- Esimerkkiohjelman rajoitukset? (`long`-tyyppi)
- Parametri vs. argumentti
- Funktion `scanf` virhetilanteet
- Esikääntäjä ja `#define` jo täällä?
- Paremmin että sama C-ohjelma toimii eri ympäristöissä (toisin kuin konekielessä)
- Funktio = aliohjelma, muita sanoja?
- Funktion otsikko (header) ja runko (body)?
- Myös funktiokutsu on lauseke
- Muuttujan näkyvyysalue paremmin (paikallinen vs. globaali)
- Tyhjä lause
- Ehdollinen lauseke: suuremman luvun valinta
- Vertailu `switch` ja Pascalin rakenne

## Luku 2

- `struct __attribute__((__packed__))` pakkaus
- offsetof makro?
- Bittikentät (bit fields)
- Mikä on `NULL`-osoitin?
- Esittele `->` jo tässä vaiheessa?
- Termi yhden komplementti?
- `a[i]` tarkoittaa samaa kuin `i[a]`

## Luku 3

- Parametria `const` voi kuitenkin muuttaa?

## Luku 4

## Luku 5

- Pythonin toteutuksiin vertaileminen?
- Paremmin taulukon käyttämisestä
  - Taulukon indeksöinti vs. `set`-rakenne
  - Järjestäminen ja binäärihaku vs. hajautus, keko, binäärihakupuu
- Taulukon enemmistöalkio?

## Luku 6

- File descriptor -> tiedoston tunniste?
- `freopen`?
- RLE-purku hienommin bitset/union avulla?
- Toimiiko tiedoston sisällön tulostus vai tarvitaanko `unsigned char`?

## Luku 7

- Esittele `#pragma once`?
- Make vai Makefile?
- Otsikkotiedosto kätevä myös koska esittelee funktiot

## Luku 8

- Komentojen määrä/yksinkertaisuus (jakolasku -> bitshift)
- Algoritmin vaikutus
- Ohjelmointikielen vaikutus
- Koodin rinnakkainen suoritus (liukuhihna) -> kertoma-esimerkki?
- Muistin käsittelyn paikallisuus
- Koodin suorituksen ennustettavuus
- Koodin profilointi työkalulla
- Kuinka tietää mitä koodi tekee oikeasti
- Loop unrolling, komentojen rinnakkaisuus, Duff's device
- Taulukkolista vs. linkitetty lista
- Liukuvan ikkunan minimit
- Funktiokutsun hitaus, inline-funktiot
- Muistiviittausten tasaus
- Silmukan purkaminen ja funktion upotus lisäävät koodin määrää

## Luku 9

- Mitä `$0x402000` tarkoittaa? Voiko katsoa myös osion `.data` sisällön?
- Kommentointi
- Miksi C:ssä `int` on 32-bittinen vaikka 64-bittistä koodia?
- Ohjelman muistin eri osien rooli: read-only, suoritettava, jne.
- Titokone
- Komennon nopeus, ennen kellosyklit, nykyään?
- Joka prosessilla on omat muistialueensa/rekisterinsä

## Luku 10

- RIP-relative addressing
- Parempi sana tiedosto-osoittimelle
- Vaihtoehdot systeemikutsuille
- Punaisen pisteen piirtäminen näytölle ennen
- Systeemikutsujen yhteys C-standardikirjastoon
- Kertomassa aliohjelmat ensin, sitten pääohjelma?
- Systeemikutsujen näyttäminen
- Bittirotaatiot?
- Esittele täällä jo komento `test`?
- Rekisterin arvojen vaihtaminen xor-trikillä
- struct ja liukuluvut

## Luku 11

- Mainitse `rip` sopivissa kohdissa
- Esimerkki joka lukee tietoa tiedostosta?

## Luku 12

- Kanarianlintu kuvitus
- Compiler Explorer (godbolt)
- http://ftp.parisc-linux.org/docs/arch/elf-64-hp.pdf
