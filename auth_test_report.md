# Authorization Test Report

## Guest

### ✅ Can do
- Näkee julkiset varaukset / -spec.8
- Pääsee /login ja /register sivulle
- Pääsee /resources sivulle ?
- Näkee varaukset /api/reservations ?
- Näkee /api/resources ?

### ❌ Cannot do
- Ei pääse katsomaan varausten tietoja eikä nää varaajaa / -spec.8
- Ei pääse /reservation sivulle
- Ei pääse /profile sivulle
- Ei pääse /admin/*

## Reserver

### ✅ Can do
- Pystyy tekemään /reservation ja /resource
- Pystyy muokkaamaan omaa varausta
- Näkee varaukset ja niiden varaajat

### ❌ Cannot do
- Ei pysty muokata muiden varauksia

## Administrator

### ✅ Can do
- Pystyy muokkaamaan ja poistamaaan varauksia -spec.4

### ❌ Cannot do
- Ei pysty poistaa käyttäjiä - spec.5
