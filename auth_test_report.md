# Authorization Test Report

## Guest

### ✅ Can do
- Näkee julkiset varaukset etusivulla / -spec.8
- Pääsee /login ja /register sivuille
- Pääsee tekemään uuden resources /resources
- Näkee varaukset listana /api/reservations ⚠️
- Näkee listana /api/resources
- Näkee käyttäjien tokenit, spostit ja roolit /api/users ⚠️

### ❌ Cannot do
- Ei pääse varauksen sivulle muokkaamaan sitä eikä nää varaajaa / -spec.8
- Ei pääse tekemään varausta /reservation
- Ei pääse /profile sivulle
- Ei pääse /admin sivulle

## Reserver

### ✅ Can do
- Pystyy tekemään /reservation ja /resource
- Näkee listattuna /api/reservations ja /api/resources
- Pystyy muokkaamaan omaa varausta ja muuttamaan varaajaa /reservation?id= ⚠️
- Näkee varaukset ja niiden varaajat /

### ❌ Cannot do
- Ei pääse muiden tekemien varausten sivulle eikä pysty muokata niitä /
- Ei pääse omalle sivulle /profile

## Administrator

### ✅ Can do
- Pystyy muokkaamaan ja poistamaaan kaikkien varauksia / -spec.4
- Pystyy tekemään uusia /reservation ja /resource

### ❌ Cannot do
- Ei pysty poistaa käyttäjiä /users/delete/:id - spec.5 ⚠️
- Ei näe käyttäjiä /admin/users -toiminnallinen virhe
