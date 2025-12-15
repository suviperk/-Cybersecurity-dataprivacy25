# Authorization Test Report

## Guest

### ✅ Can do
- Näkee julkiset varaukset / -spec.8
- Pääsee /login ja /register sivulle
- Pääsee /resources sivulle 
- Näkee varaukset /api/reservations 
- Näkee /api/resources 

### ❌ Cannot do
- Ei pääse katsomaan varausten tietoja eikä nää varaajaa / -spec.8
- Ei pääse /reservation sivulle
- Ei pääse /profile sivulle
- Ei pääse /admin/*

## Reserver

### ✅ Can do
- Pystyy tekemään /reservation ja /resource
- Näkee /api/reservations ja /api/resources
- Pystyy muokkaamaan omaa varausta ja muuttamaan varaajaa /reservation?id=
- Näkee varaukset ja niiden varaajat /

### ❌ Cannot do
- Ei pysty muokata muiden varauksia /
- Ei pääse omalle sivulle /profile

## Administrator

### ✅ Can do
- Pystyy muokkaamaan ja poistamaaan kaikkien varauksia / -spec.4
- Pystyy tekemään /reservation ja /resource

### ❌ Cannot do
- Ei pysty poistaa käyttäjiä /users/delete/:id - spec.5
