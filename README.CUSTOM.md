## Verdrahtung (TH05Y_V3.1)

<img width="3072" height="4080" alt="PXL_20261018_111022120" src="https://github.com/user-attachments/assets/0a66439f-5abf-4ef1-9415-0f4f211f1069" />
<img width="3072" height="4080" alt="PXL_20261018_111013568" src="https://github.com/user-attachments/assets/b287b811-9339-4fb5-a7b8-4124959f7f30" />

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
5. Sofort danach `python3 rdwr_phy62x2.py -p /dev/ttyUSB0 -e -r wh ./bin/BOOT_TH05F_v21.hex` ausführen (ohne TM angeschlossen)
   Oder `python3 rdwr_phy62x2.py -p /dev/cu.usbserial-11320 -t -e -r wh ./bin/BOOT_TH05F_v21.hex` (mit TM angeschlossen)

Flashvorgang sollte laufen


## Prüfen auf welchem Port der Adapter läuft
`ls /dev/cu.*`
