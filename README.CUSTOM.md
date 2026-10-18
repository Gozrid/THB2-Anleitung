## Verdrahtung (TH05Y_V3.1)

|Adapter|Sensor|
|---|---|
|3V3|VBAT+; TM|
|TXD|RX1|
|RXD|TX1|
|GND|VBAT-; REST_N|

## Programmierung
1. Python Virtual Environment erstellen: `python3 -m venv .venv`
2. Python Virtual Environment nutzen: `source ./.venv/bin/activate`
3. Bibliotheken installieren: `pip install -r requirements.txt`
4. RESET an GND halten um zu resetten
5. Sofort danach `python3 rdwr_phy62x2.py -p /dev/ttyUSB0 -e -r wh ./bin/BOOT_TH05F_v21.hex` ausführen

Flashvorgang sollte laufen


## Prüfen auf welchem Port der Adapter läuft
`ls /dev/cu.*`
