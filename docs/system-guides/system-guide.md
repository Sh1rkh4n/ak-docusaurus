---
sidebar_position: 1
---

# Általános információk

:::info[**Információ**]

A rendszer angol és magyar nyelven érhető el, amely a felhasználói profilban módosítható.

:::

## Belépés a rendszerbe

A rendszerre történő bejelentkezés a login felületén történik M-es azonosítóval és ActiveDirectory jelszóval. A rendszer 5 percen belüli 5 sikertelen bejelentkezési kísérlet után kizárja a felhasználót 15 percre.

## Navigáció és beállítások

A képernyő három részre bontható : 1 Menü, 2 Navigációs panel, 3 Megjelenítési felület.

### Menü

- **Céges logó/Kezdőoldal:** Átirányít a kezdőoldalra
- **Csengő ikon/Értesítések:**   Megnyitja az értesítések listáját
- **Felhasználó avatar és adatok:**  A bejelentkezett felhasználó neve és avatarja
- **Felhasználó ikon/Beállítások:** Felugró ablakban megnyitja a felhasználói beállításoakt
- **Segítség ikon:** Felugró ablakban megnyitja a fejlesztő csapat elérhetőségeit és néhány információt a rendszerről
- **3 pont:** Kijelentkezés és főoldalra ugrás lehetősége

### Navigációs sáv

- A kinyitható oldalsáv tartalmaz minden elérhető modult az oldalon funkciónként csoportosítva.

- A három vízszintes vonalra kattintva a menü kinyitható, a funkciókra kattintva megjelennek az odatartozó modulok. Rájuk kattintva az oldal elnavigál a megfelelő felületre.

### Megjelenítési felület

Ez az oldal fő felülete. Itt jelennek meg a kiválasztott modulok. A rendszer indításakor a megjelenítési felület automatikusan a kezdőoldalt mutatja.

### Kommentek és megjegyzések

A kommentek és feljgyzések kerülnek ebbe a fejezetbe.

## Felhasználó kezelés

Az oldalmenüben kattints a User Role Management gombra, ekkor megjelennek az elérhető modulok : User Manager, Group Management, Manage Group Members.

- **Felhasználó Kezelő Manager** : megfelelő jogosultsággal itt tudod engedélyezni és korlátozni a felhasználókat, lezárni/feloldani a fiókokat és új felhasználókat importálni WorkDay-es adatok alapján.
- **Csoport Kezelő** : megfelelő jogosultsággal itt tudod módosítani a felhasználói csoportok leírását.
- **Tagság Kezelő** megfelelő jogosultsággal itt tudsz hozzáadni felhasználókat a csoportokhoz vagy eltávolítani őket onnan.

### Felhasználó kezelő

Ezen a felületen láthatod a rendszerben elérhető felhasználók listáját. Zöld pipával és piros X ikonnal jelölve látható hogy a felhasználó elérhető-e, zárolt-e. A lista felett található  szűrő  segítségével kereshetsz a listában felhasználó név vagy e-mail cím alapján.

- Sor kiválasztásával elérhetővé tehetsz/zárolhatsz fiókokat.

- Az Export gombra kattintva elmentheted a felhasználók listáját egy excel fileban.

- Az Import Users gombra kattintva felhasználókat importálhatsz.

#### Felhasználók importálása

- Felhasználók importálásához kattints az ‘Import Users’ gombra.
- Húzd a WorkDay riport .csv file-t a felugró ablakra vagy kattints a gombra a file kiválasztásához, majd kattints az ‘Upload’ gombra.
- Egy felugró státuszüzenet értesít a sikeres importról.

#### Felhasználó engedélyezése, zárolása

- Kattintással válaszd ki a felhasználót a listából.
- A jelölőnégyzet segítségével végezd el a kívánt változtatásokat.
- Kattints a mentés gombra a változtatások véglegesítéséhez.

### Group Management / Csoport kezelő

Ezen a felületen módosíthatod a Felhasználói Csoportok leírását és láthatod a rekordokon végzett módosításokat. Az ‘Open Comments’ gombra kattintva írhatsz és olvashatsz a csoportokhoz kapcsolódó megjegyzéseket.

**Csoport leírásának megváltoztatásához :**

- A legördülő menüből válassz ki egy csoportot.
- Módosítsd a leírást a lista alatti szövegmezőben. A leírásnak 10 és 500 közötti hosszúságúnak kell lennie és csak betűket, számokat és ‘ – ‘, ‘ . ‘, ‘\_’ és ‘,’ karaktereket tartalmazhat.
- Menteni a  ‘Save’ gomb megnyomásával tudsz.

### Csoporttagság kezelő

Ezen az oldalon Felhasználókat adhatsz hozzá Csoportokhoz vagy távolíthatod el őket onnan.

**Felhasználók hozzáadása csoporthoz :**

- Válassz ki egy csoportot a legördülő listából.
- Válaszd ki a hozzáadni kívánt felhasználókat kattintással a bal oldali listából majd nyomj az ‘Add’ gombra.
- A módosításokat a ‘Save’ gombra kattintva mentheted el.

**Felhasználók eltávolítása csoportból :**

- Válassz ki egy csoportot a legördülő listából.
- Válaszd ki az eltávolítani kívánt felhasználókat kattintással a jobb oldali listából majd nyomj a ‘Remove’ gombra.
- A módosításokat a ‘Save’ gombra kattintva mentheted el.

### Jogosultságok

**Jogosultságok ellenőrzése:**

- Válaszd ki a csoportot a Csoportok Listából
- Válaszd ki a Mashup-ot a Mashupok Listájából

Frissítheted az adatokat a ’Frissítés’ gombbal.

## Ellenőrzési Napló

Az oldalsávon kattints az Audit Trail feliratra, ekkor megjelennek az elérhető modulok: Audit Tábla Adatok, Biztonsági Események:

- Audit Tábla Adatok: Megjeleníti az összes Audit Napló bejegyzést.
- Biztonsági Események: Megjeleníti a Biztonsági Napló bejegyzéseit.