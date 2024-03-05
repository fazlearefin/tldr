# mdk4

> MDK4 is a proof-of-concept tool to exploit common IEEE 802.11 protocol weaknesses.
> (Exercise caution when utilizing MDK4 for security testing to prevent unauthorized activities or disruptions.)
> More information: <https://github.com/aircrack-ng/mdk4>.

- Send beacon frames to generate a fake AP (Access Point):

`mdk4 b -n {{SSID}}`

- Send beacon frames to show many fake APs at clients (may crash certain devices in range):

`mdk4 b`

- Send deauthentication and disassociation packets to stations based on data traffic to disconnect all clients from an AP:

`mdk4 d`
