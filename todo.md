---
title: TODO
permalink: /todo
hide: true
---

# TODO

## Tärkeää tehtävää pian

- Lue C-standardeja
- Kaikkien lukujen johdantotekstit
- Esimerkkitulosteiden kieli englanniksi
- Mieti miten esittää pitkän koodin analyysi osissa hyvin
- Mainitse että tavuesitykset ovat materiaalissa yleisesti heksalukuina
- Pystyykö korjaamaan ongelmat koodin/konsolin värityksessä?
- Käytä `size_t` oikeissa paikoissa
- Lippu `-O2` sopivassa kohdassa
- Luku 1: käsittele esikääntäjää

## Yleistä

- Paluuarvo vai palautusarvo?
- Virtuaalinen muisti vs. fyysinen muisti, tuo esille usein
- Rakenne `enum`
- Mitkä parametrit käännöksessä? (`-Wall`, `-Wextra`, `-O2`, `-std=c99`, `-pedantic`)
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
- `getchar`, `putchar`, `gets`, `puts`
- `int` oletustyyppi, jäänne `unsigned` = `unsigned int`
- `int*` tarkoittaa sekä osoite yhteen lukuun että taulukkoon
- Mitä `#include` oikeastaan tekee?
- Avainsana `volatile`?
- Esittele mielekäs osa tiedostosta `stdio.h`?
- `return x - y` ei toimi oikein järjestämisessä?
- Kaikki koodiesimerkkien tulostukset englanniksi?
- Yhdenmukaisesti arvot: 42 vai `42`
- Tarkasta kuvien skaalausta (ainakin luvussa 2)
- Tarkasta että console käytetty kaikissa tulostusesimerkeissä
- Toteuta merkkijonojen yms. läpikäynti C-tyylisesti
- Voiko kurssimateriaalin koodimerkinnän värityksiä korjailla?
- Binääritiedosto, ohjelmatiedosto vai mikä nimi?
- Komento continue jonnekin?
- C-kielen yhteys PDP-11-konekieleen
- Inline assemblyn syntaksi

## Luku 1

- Operaattoreiden presedenssi
- Lausekkeen osien suoritusjärjestys (and, or)
- Suoritusjärjestys ei aina selvä
- Duff's device? tai muuten switch tarkemmin
- Esimerkkiohjelman rajoitukset? (`long`-tyyppi)
- Parametri vs. argumentti
- Funktion `scanf` virhetilanteet
- Kääntäjä varoittaa jos `scanf`-funktion palautusarvoa ei käsitellä
- Esikääntäjä ja `#define` jo täällä?
- Paremmin että sama C-ohjelma toimii eri ympäristöissä (toisin kuin konekielessä)
- Funktion otsikko (header) ja runko (body)?
- Myös funktiokutsu on lauseke
- Muuttujan näkyvyysalue paremmin (paikallinen vs. globaali)
- Muut C:n aikalaiskielet, historiallinen tausta
- Muuttujan näkyvyysalue: kuitenkin vasta määrittelyn jälkeen lohkossa
- Parempi esimerkki goto-komennosta monikerroksisessa silmukassa
- Kerro kielten eroista arvoparametrien ja viittausparametrien käytössä

## Luku 2

- Tyyppi `long long` mukaan vai ei?
- Miksi kahden komplementtia käytetään?
- offsetof makro?
- Bittikentät (bit fields)
- Mikä on `NULL`-osoitin?
- Termi yhden komplementti?
- `a[i]` tarkoittaa samaa kuin `i[a]`
- Ennen structia voisi kertoa jo tiedon kohdistuksesta muistissa ja muistiosoitteista vähän tarkemmin
- Pinon sijainti muistissa ja tietoturva

## Luku 3

- Parametria `const` voi kuitenkin muuttaa?
- Merkkikoodit unsigned-arvoina UTF-8-esimerkissä?

## Luku 4

- Avainsanan `auto` uusi käyttö C23-standardissa

## Luku 5

- Virheenkäsittely tietorakenteisiin?
- Parempi hajautustapa kuin lineaarinen kokeilu, tai ainakin tuo esille ettei hyvä
- Pythonin toteutuksiin vertaileminen?

## Luku 6

- File descriptor -> tiedoston tunniste?
- `freopen`?
- RLE-purku hienommin bitset/union avulla?

## Luku 7

- Esittele `#pragma once`?
- Otsikkotiedosto kätevä myös koska esittelee funktiot

## Luku 8

- Muistiviittausten tasaus
- Taulukkolista vs. linkitetty lista
- Optimointi on huono sana?
- Testiaineisto?

## Luku 9

- Miksi C:ssä `int` on 32-bittinen vaikka 64-bittistä koodia?
- Titokone
- Komennon nopeus, ennen kellosyklit, nykyään?
- Joka prosessilla on omat muistialueensa/rekisterinsä
- Historialliset arkkitehtuurit, kuten PDP-11

## Luku 10

- Parempi sana tiedosto-osoittimelle
- Systeemikutsujen yhteys C-standardikirjastoon
- Bittirotaatiot?
- struct ja liukuluvut
- mikä tarkalleen erona `mov rax, number` ja `lea rax, [number]` (32-bittinen vs. 64-bittinen osoite)
- tarkemmin osoitteiden käsittelystä (hyppykomennot, lea ja rel)

## Luku 11

- Esimerkki joka lukee tietoa tiedostosta?
- Kolmas esimerkki funktion toteuttamisesta?

## Luku 12

- Voisi korvata "and eax, 1 -- test rax, rax" komennolla "test rax, 1"?
- Käytännön esimerkki IBT:stä sekä miksi IBT ei käytössä?
- Kanarianlintu kuvitus
- Kerro paremmin `add rax, 1` ja `inc rax` erosta
