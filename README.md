# ATX2xBeezy
This project allows you to convert an ATX PSU to work as a 213W XB Power Supply.

Features:
- 3A current limiting on the 5V rail to protect console/sidecar circuitry from short circuits or over current scenarios (based around the [TCKE920NL](https://toshiba.semicon-storage.com/info/TCKE920NL_datasheet_en_20250819.pdf?did=157593&prodName=TCKE920NL) IC)
- Allows console to trigger 12V rail as requested via MOSFET and relay
- Allows for Raspberry Pi Pico to be used to safely shutdown the PSU via ATX_EN pin (Pull high to enable the ATX PSU, pull low to disable).
- Allows for monitoring of 5V rail via PWR_GD line (High state indicates the 5V rail is operating normally, low state indicates U1 is in fault state and OCP has been triggered)


<img width="1724" height="930" alt="Top Down View" src="https://github.com/user-attachments/assets/152a5e95-d7d9-4134-ad03-09e2fab8625e" />

<img width="1724" height="930" alt="Side View" src="https://github.com/user-attachments/assets/50844cba-5a87-4345-9dca-394f7e15831e" />

<img width="1724" height="930" alt="Bottom View" src="https://github.com/user-attachments/assets/a74775bf-b412-4ccc-a4e1-ca30048d501e" />
