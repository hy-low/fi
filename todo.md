---
title: TODO
permalink: /todo
hide: true
---

# TODO

## Tärkeää tehtävää pian

- Kaikkien lukujen johdantotekstit
- Esimerkkitulosteiden kieli englanniksi
- Muuta `switch` -> switch jne.?
- Käytä `size_t` oikeissa paikoissa
- Luku 1: käsittele esikääntäjää
- Luku 1: laskujärjestys ja muut asiat lausekkeissa
- Luku 1: main-funktion palautusarvo loppuun
- Luku 2: rakenteinen vs. perustietotyyppi
- Luku 2: syntaksi kentän käsittelyyn osoittimen kautta
- Luku 2: rakenteisen tietotyypin muistinvaraus
- Luku 5: lisää virheenkäsittely tietorakenteisiin
- Luku 5: syntaksi `->` käyty tulevaisuudessa jo aiemmin
- Luku 5: `array_list_print` ei toimi järkevästi yleisessä toteutuksessa -> käytä mieluummin `array_list_get` pääfunktiossa?
- Luku 5: taulukon vahvuudet

## Yleistä

- Paluuarvo vai palautusarvo?
- Virtuaalinen muisti vs. fyysinen muisti, tuo esille usein
- Rakenne `enum`
- Mitkä parametrit käännöksessä? (`-Wall`, `-Wextra`, `-O2`, `-std=c99`, `-pedantic`)
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
- Avainsana `volatile`?
- Esittele mielekäs osa tiedostosta `stdio.h`?
- `return x - y` ei toimi oikein järjestämisessä?
- Kaikki koodiesimerkkien tulostukset englanniksi?
- Rakenteiden nimet: `switch`-rakenne vai switch-rakenne?
- Yhdenmukaisesti arvot: 42 vai `42`
- Tarkasta kuvien skaalausta (ainakin luvussa 2)
- Tarkasta että console käytetty kaikissa tulostusesimerkeissä
- Toteuta merkkijonojen yms. läpikäynti C-tyylisesti

## Luku 1

- Operaattoreiden presedenssi
- Lausekkeen osien suoritusjärjestys (and, or)
- Suoritusjärjestys ei aina selvä
- Duff's device? tai muuten switch tarkemmin
- Esimerkkiohjelman rajoitukset? (`long`-tyyppi)
- Parametri vs. argumentti
- Funktion `scanf` virhetilanteet
- Esikääntäjä ja `#define` jo täällä?
- Paremmin että sama C-ohjelma toimii eri ympäristöissä (toisin kuin konekielessä)
- Funktion otsikko (header) ja runko (body)?
- Myös funktiokutsu on lauseke
- Muuttujan näkyvyysalue paremmin (paikallinen vs. globaali)
- Muut C:n aikalaiskielet, historiallinen tausta
- Muuttujan näkyvyysalue: kuitenkin vasta määrittelyn jälkeen lohkossa
- Käsittele paremmin for-silmukka
- Parempi esimerkki goto-komennosta monikerroksisessa silmukassa
- Kerro kielten eroista arvoparametrien ja viittausparametrien käytössä

## Luku 2

- Tyyppi `long long` mukaan vai ei?
- Miksi kahden komplementtia käytetään?
- `struct __attribute__((__packed__))` pakkaus
- offsetof makro?
- Bittikentät (bit fields)
- Mikä on `NULL`-osoitin?
- Esittele `->` jo tässä vaiheessa?
- Termi yhden komplementti?
- `a[i]` tarkoittaa samaa kuin `i[a]`

## Luku 3

- Parametria `const` voi kuitenkin muuttaa?
- Merkkikoodit unsigned-arvoina UTF-8-esimerkissä?

## Luku 4

- Avainsanan `auto` uusi käyttö C23-standardissa

## Luku 5

- Parempi hajautustapa kuin lineaarinen kokeilu?
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

- Ohjelmointikielen vaikutus
- Kuinka tietää mitä koodi tekee oikeasti
- Muistiviittausten tasaus
- Silmukan purkaminen ja funktion upotus lisäävät koodin määrää
- Taulukkolista vs. linkitetty lista

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

- Tarkasta käännetyt koodit (puuttuvia arvojen kokoja?)
- Kanarianlintu kuvitus
- Compiler Explorer (godbolt)
- http://ftp.parisc-linux.org/docs/arch/elf-64-hp.pdf
