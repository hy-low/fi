---
title: TODO
permalink: /todo
hide: true
---

# TODO

## Tärkeää tehtävää pian

- Pystyykö korjaamaan ongelmat koodin/konsolin värityksessä?

## Yleistä

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
- Pino kasvaa alaspäin eikä oikealta vasemmalle

## Luku 1

- Duff's device? tai muuten switch tarkemmin
- Esimerkkiohjelman rajoitukset? (`long`-tyyppi)
- Parametri vs. argumentti
- Funktion `scanf` virhetilanteet
- Kääntäjä varoittaa jos `scanf`-funktion paluuarvoa ei käsitellä
- Paremmin että sama C-ohjelma toimii eri ympäristöissä (toisin kuin konekielessä)
- Funktion otsikko (header) ja runko (body)?
- Muut C:n aikalaiskielet, historiallinen tausta
- Muuttujan näkyvyysalue: kuitenkin vasta määrittelyn jälkeen lohkossa
- Parempi esimerkki goto-komennosta monikerroksisessa silmukassa
- Kerro kielten eroista arvoparametrien ja viittausparametrien käytössä
- goto kuuluu samaan ryhmään kuin break, continue, return?

## Luku 2

- offsetof makro?
- Bittikentät (bit fields)
- Mikä on `NULL`-osoitin?
- `a[i]` tarkoittaa samaa kuin `i[a]`
- Ennen structia voisi kertoa jo tiedon kohdistuksesta muistissa ja muistiosoitteista vähän tarkemmin
- Pinon sijainti muistissa ja tietoturva
- Osoittimen käyttö ei tehosta pienien structien kopiointia

## Luku 3

- Parametria `const` voi kuitenkin muuttaa?
- Tarkasta mitä strncpy ja strncat tekee oikeasti

## Luku 4

- Avainsanan `auto` uusi käyttö C23-standardissa
- Miksi pinolle näkyy vain 132 kt muistia varattuna?

## Luku 5

- Virheenkäsittely tietorakenteisiin?
- Parempi hajautustapa kuin lineaarinen kokeilu, tai ainakin tuo esille ettei hyvä
- Pythonin toteutuksiin vertaileminen?
- Tarkemmin linkitetyn listan tehokkuudesta: lisäys/poisto nopea vain jos kohta on tiedossa
- `strdup` ei ole standardikirjaston funktio?
- Bugi `if (i - deque[left] == m) left++`

## Luku 6

- File descriptor -> tiedoston tunniste?
- `freopen`?
- RLE-purku hienommin bitset/union avulla?

## Luku 7

- Esittele `#pragma once`?
- Otsikkotiedosto kätevä myös koska esittelee funktiot
- Näkyvyys tiedostoissa vs. sisäinen ja ulkoinen linkitys

## Luku 8

- Taulukkolista vs. linkitetty lista
- Optimointi on huono sana?
- Testiaineisto?
- `-Os` muistuttaa `-O2` mutta osa optimoinneista puuttuu
- Tässäkin deque-bugi

## Luku 9

- Miksi C:ssä `int` on 32-bittinen vaikka 64-bittistä koodia?
- Titokone
- Komennon nopeus, ennen kellosyklit, nykyään?
- Joka prosessilla on omat muistialueensa/rekisterinsä
- Historialliset arkkitehtuurit, kuten PDP-11
- Älä käytä `nasm` silloin kun ei ole NASM-koodia?

## Luku 10

- Parempi sana tiedosto-osoittimelle
- Systeemikutsujen yhteys C-standardikirjastoon
- Bittirotaatiot?
- struct ja liukuluvut
- mikä tarkalleen erona `mov rax, number` ja `lea rax, [number]` (32-bittinen vs. 64-bittinen osoite)
- tarkemmin osoitteiden käsittelystä (hyppykomennot, lea ja rel)
- `read_number`: rekisterin `rdx` käyttö epämääräistä
- `syscall` tuhoaa `rcx` ja `r11`?
- `read_number` voisi käyttää palautettua tavumäärää

## Luku 11

- Esimerkki joka lukee tietoa tiedostosta?
- Kolmas esimerkki funktion toteuttamisesta?
- Rekursiivinen `fibo` ei tasaa pinoa
- `fibo` myös ero `int` vs. 64-bittiset arvot

## Luku 12

- Voisi korvata `and eax, 1 -- test rax, rax` komennolla `test rax, 1` tai vain `and eax, 1`?
- Käytännön esimerkki IBT:stä sekä miksi IBT ei käytössä?
- Kanarianlintu kuvitus
- Kerro paremmin `add rax, 1` ja `inc rax` erosta
- Assembly-koodi käsin muokattua eikä yhtenäistä
- Kanarialintu tulee `scanf`-funktion takia?
- Kanarialintu suojaa vain tilannetta jossa puskuriylivuoto menee tarpeeksi pitkälle
- `endbr64` liittyy yleisemmin ehdolliseen haarautumiseen, ei vain aliohjelmiin
- Mikä on `__printf_chk`
- Kääntäjän toiminta riippuvainen ympäristöstä/asetuksista
