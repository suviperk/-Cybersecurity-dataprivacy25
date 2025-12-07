# Password Cracking – Phase 2

## 1. Murretut salasanat

Käytin tehtävässä työkaluna: John the Ripper
Ja käyttäen sanalistaa `rockyou.txt`:

| Salasana |
|----------|
| iamironman |
| carrots123 |
| donuts4life |
| darkside42 |
| ...       |

## 2. Screenshot murtamisesta

![Johnin tulokset](kuva.PNG)


## 3. Teoriakysymykset

### 3.1 Mikä ero on dictionary- ja non-dictionary-hyökkäyksillä?

- **Dictionary attack:** kokeillaan valmiista sanalistasta löytyviä salasanoja, nopea jos salasana on yleinen.
- **Non-dictionary (brute-force):** kokeillaan kaikkia mahdollisia yhdistelmiä, hidas mutta varma tapa löytää mikä tahansa salasana.

### 3.2 Hyöty, jos hyökkääjä saa hashit ja käyttäjätiedot

- Hashien avulla salasanoja voi murtaa offline.
- Ei tarvita käyttäjän järjestelmää.
- Pääsee käsiksi käyttäjätileihin, kun salasana murretaan.

### 3.3 Pitkien salasanojen hyödyt

- Lisää merkittävästi mahdollisia yhdistelmiä → vaikeampi murtaa brute-force‑menetelmällä.
- Pidemmät salasanat tarjoavat enemmän entropyä → turvallisemmat.

