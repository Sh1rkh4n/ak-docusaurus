---
sidebar_position: 1
title: Telepítési Útmutató
description: ThingWorx Telepítési Útmutató
---

---

### ⚙️ **ThingWorx Telepítési Útmutató – `thingworx-telepites.md`**

::::info

Ez a dokumentum lépésről lépésre bemutatja a ThingWorx Foundation szerver telepítését.

::::

## Előfeltételek

- Java Development Kit (JDK) 11 vagy 17
- Apache Tomcat 9 vagy 10
- ThingWorx Foundation WAR fájl
- ThingWorx Platform licencfájl
- PostgreSQL vagy Microsoft SQL Server adatbázis
- 64-bit operációs rendszer (Windows vagy Linux)

## 1. Java és Tomcat telepítése

1. Telepítsd a JDK-t (ajánlott JDK 11 vagy JDK 21).
2. Állítsd be a `JAVA_HOME` környezeti változót.
3. Telepítsd az Apache Tomcat szervert.
4. Másold a `thingworx.war` fájlt a Tomcat `webapps` mappájába.

## 2. PlatformStorage és Repositories könyvtárak létrehozása

1. Hozd létre a következő mappákat a Tomcat gyökérkönyvtárban (pl. `C:\ThingworxStorage` és `C:\ThingworxPlatform`).
2. Helyezd el a licencfájlt (`license_capability_response.bin`) a `ThingworxPlatform` mappába.

## 3. Adatbázis beállítása

1. Hozz létre egy adatbázist pl. `thingworx` néven.
2. Hozz létre egy dedikált felhasználót jelszóval.
3. Engedélyezd a szükséges jogosultságokat (`CREATE`, `SELECT`, `INSERT`, stb.).
4. Töltsd ki a `platform-settings.json` fájlt az adatbázis csatlakozáshoz (ld. következő fájl).

## 4. Tomcat konfigurálása

1. Állítsd be a `CATALINA_OPTS` értékét pl.:

   ```shell
   -Xms512m -Xmx4g -Dfile.encoding=UTF-8 -Djava.library.path="C:\ThingworxStorage"
   ```
