# DEALER

Statikus, szerver nélküli böngészős játékgyűjtemény. Nincs build-lépés a
weboldalakhoz — minden HTML fájl önmagában is megnyitható böngészőben.

- `index.html` — DEALER főmenü, innen választható ki a két játék
- `zsetonszamolo.html` — Zsetonszámoló: az asztalon lévő zsetontornyok
  értékének összeadása, 3 nehézségi szinttel (5 zseton-címlet: 100–25000)
- `emlekezet_elterelas.html` — Emlékezet & Elterelés: egy szám megjegyzése
  zavaró matekfeladatok közben (Brown–Peterson paradigma), Alap és Nehéz
  szinttel

## Android app

A `android/` mappa egy Capacitor-alapú Android csomagolás ugyanezekhez a
weboldalakhoz, "DEALER" néven, saját zseton-ikonnal és indítóképernyővel.

```
npm install
npm run sync          # weboldalak (www/) szinkronizálása az Android projektbe
npm run open:android  # projekt megnyitása Android Studio-ban
```

Android Studio-ban onnan futtatható emulátoron/telefonon (▶ Run), vagy
`assembleDebug` Gradle taskkal telepíthető APK készíthető.
