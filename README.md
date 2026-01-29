# domoticz-ada-p1-meter

Python plugin for Domoticz to integrate the ADA P1 Meter smart energy meter
(imported / exported energy, tariffs, power values). 
https://greenhess.com/p1-meter

# Prerequisites

- Domoticz 2022.1 or newer

- Domoticz with Python plugin support enabled
https://www.domoticz.com/wiki/Using_Python_plugins

# Installation

You can install the plugin manually or by using the
[Domoticz Plugins Manager](https://github.com/stas-demydiuk/domoticz-plugins-manager)

## Manual installation

1. Clone or copy the plugin into your Domoticz plugins directory:
    ```
    cd domoticz/plugins
    git clone https://github.com/szelessavalapitvany/ADA_P1_meter_for_Domoticz
    ```
2. Restart Domoticz
3. Make sure “Accept new Hardware Devices” is enabled in Domoticz settings
4. Go to Setup → Hardware
5. Add a new hardware device with type “ADA P1 Meter"
6. Configure the required parameters:

    * communication method (MQTT / LAN / serial – depending on plugin version)
    * IP address, port, topic, or other connection settings

## Plugin update

1. Go to the plugin directory and pull the latest version:
```
cd domoticz/plugins/ADA_P1_Meter
git pull
```
2. Restart Domoticz

Note:
If you modified plugin files and git pull fails, you can stash local changes:
```
git stash
```
## Plugin downgrade

1. Reset the plugin to an earlier version:
    ```
    cd domoticz/plugins/ADA_P1_Meter
    git reset --hard <commit_hash>
    ```
2. Restart Domoticz
(or disable and re-enable the plugin under Setup → Hardware; browser cache cleanup may be required)
---
---
# domoticz-ada-p1-meter (magyarul)

Python plugin Domoticzhoz, amely az ADA P1 Meter okosmérő integrációját valósítja meg
(importált / exportált energia, tarifák, teljesítmény adatok).
https://greenhess.com/p1-meter

# Előfeltételek

- Domoticz 2022.1 vagy újabb

- Python plugin támogatás engedélyezve a Domoticzban
https://www.domoticz.com/wiki/Using_Python_plugins

# Telepítés

A plugin telepíthető manuálisan vagy a
[Domoticz Plugins Manager](https://github.com/stas-demydiuk/domoticz-plugins-manager) segítségével.

## Manuális telepítés

1. Másold / klónozd a plugint a Domoticz plugin könyvtárába:
    ```
    cd domoticz/plugins
    git clone https://github.com/szelessavalapitvany/ADA_P1_meter_for_Domoticz
    ```
2. Indítsd újra a Domoticzot
3. Ellenőrizd, hogy az „Accept new Hardware Devices” engedélyezve van
4. Lépj a Setup → Hardware menübe
5. Add hozzá az új hardvert „ADA P1 Meter” típussal
6. Állítsd be a szükséges paramétereket:

    * kommunikáció módja (MQTT / LAN / soros – a plugin verziójától függően)
*   IP cím, port, topic vagy egyéb kapcsolódási adatok

## Plugin frissítése

1. Lépj be a plugin könyvtárába és frissítsd:
```
cd domoticz/plugins/ADA_P1_Meter
git pull
```
2. Indítsd újra a Domoticzot

Megjegyzés:
Ha módosítottad a plugin fájljait és a git pull nem fut le, a helyi változtatások eltárolhatók:
```
git stash
```
### Plugin visszaléptetése (downgrade)

1. Régebbi verzió visszaállítása:
    ```
    cd domoticz/plugins/ADA_P1_Meter
    git reset --hard <commit_hash>
    ```
2. Domoticz újraindítása
(vagy a plugin letiltása majd újra engedélyezése a Setup → Hardware menüben; böngésző cache törlés szükséges lehet)
