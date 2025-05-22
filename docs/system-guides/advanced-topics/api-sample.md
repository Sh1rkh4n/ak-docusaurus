---
sidebar_position: 2
title: API Dokumentáció – Integrációs Példa
---

## Áttekintés

Ez a dokumentáció bemutat egy REST alapú API integrációs példát, amely lehetővé teszi külső rendszerek számára adatok lekérdezését és frissítését.

Általános leírást az alábbi helyen talál: [#API Integráció](/docs/system-guides/advanced-topics/api-integration.md).

---

## Hitelesítés

Minden API kéréshez szükséges egy érvényes API kulcs.

**Fejléc példa:**

```bash
Authorization: Bearer {API_KULCS}
```

---

## Alap URL

```bash
https://api.pelda.hu/v1
```

---

## Végpontok

### 1. Lekérdezés: Felhasználók listázása

**GET** `/users`

**Kérés példa:**

```bash
GET /v1/users HTTP/1.1
Host: api.pelda.hu
Authorization: Bearer {API_KULCS}
```

**Válasz:**

```json
[
  {
    "id": 1,
    "nev": "Kiss Gábor",
    "email": "gabor.kiss@pelda.hu"
  },
  {
    "id": 2,
    "nev": "Nagy Anna",
    "email": "anna.nagy@pelda.hu"
  }
]
```

### 2. Új felhasználó létrehozása

**POST** `/users`

**Törzs:**

```json
{
  "nev": "Tóth Ádám",
  "email": "adam.toth@pelda.hu"
}
```

**Válasz:**

```json
{
  "id": 3,
  "uzenet": "Felhasználó sikeresen létrehozva."
}
```

### 3. Felhasználó frissítése

**PUT** `/users/{id}`

**Törzs:**

```json
{
  "email": "uj.email@pelda.hu"
}
```

**Válasz:**

```json
{
  "uzenet": "Felhasználó frissítve."
}
```

### 4. Felhasználó törlése

**DELETE** `/users/{id}`

**Válasz:**

```json
{
  "uzenet": "Felhasználó törölve."
}
```

---

## Hibakódok

| Kód | Leírás                     |
|-----|----------------------------|
| 200 | Sikeres kérés             |
| 201 | Létrehozva                |
| 400 | Hibás kérés               |
| 401 | Nincs jogosultság         |
| 404 | Nem található             |
| 500 | Szerverhiba               |

---

## Kapcsolat

További információért kérjük lépjen kapcsolatba a fejlesztői csapattal: [dev@pelda.hu](mailto:dev@pelda.hu)

---

*Ez egy példa API dokumentáció markdown formátumban integrációhoz.*
