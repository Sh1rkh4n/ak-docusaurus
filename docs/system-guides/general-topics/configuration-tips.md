---
sidebar_position: 2
title: Konfigurációs Útmutató
description: ThingWorx Konfigurációs Útmutató
---

---

## ⚙️ **ThingWorx Konfiguráció – `thingworx-konfiguracio`**

Ez a dokumentum bemutatja a ThingWorx alapvető konfigurációját a `platform-settings.json` rendszerfájl segítségével.

## 1. `platform-settings.json` szerkezete

::::tip

Helye: `ThingworxPlatform/platform-settings.json`

::::

**Példa `platform-settings.json` fájl:**

```json
{
  "PlatformSettingsConfig": {
    "Storage": {
      "PersistenceProviderPackageConfigs": {
        "PostgresPersistenceProviderPackage": {
          "ConnectionInformation": {
            "jdbcUrl": "jdbc:postgresql://localhost:5432/thingworx",
            "username": "twadmin",
            "password": "jelszo"
          },
          "maxConnections": 100,
          "validationTimeout": 30000
        }
      }
    },
    "Licensing": {
      "Features": {
        "AnalyticsServer": true,
        "ManufacturingApps": false
      }
    }
  },
  "BasicSettings": {
    "EnableSystemLogging": true,
    "EnableAuditLogging": false,
    "ScriptTimeout": 60
  },
  "ContentDelivery": {
    "AllowNonSecureConnections": false
  }
}
```

---

:::note

További segítséget a program konfigurációjával vagy működésével kapcsolatosan az alábbi weboldalon talál:

>**[Thingworx - PTC - Support](https://www.ptc.com/en/support/help/Thingworx)**

:::
