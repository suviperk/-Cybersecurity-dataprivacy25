# Authorization Test Report

## Guest

### ✅ Can do
- Näkee julkiset resources/reservation
- Pääsee /login sivulle
- Pääsee /register sivulle

### ❌ Cannot do
- Ei pääse katsomaan resources tietoja eikä nää varaajaa
- Ei voi tehdä resources/reservation

## Reserver

### ✅ Can do
- Pystyy tekemään reservation tai resource
- Pystyy muokkaamaan omaa reservation
- Näkee reservation ja niiden varaajat

### ❌ Cannot do
- Ei pysty muokata muiden reservation

## Administrator

### ✅ Can do
- Pystyy muokkaamaan ja poistamaaan reservation

### ❌ Cannot do
- Ei pysty poistaa käyttäjiä
