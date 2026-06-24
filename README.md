# Glomar

Small radios, mostly. Embedded RF and wireless security, plus the telephony, mesh, and
scanner plumbing around it. ESP32, LoRa, SIP, Meshtastic. And a cat, allegedly.


### Telephony
- [pocket-dial](https://github.com/GlomarGadaffi/pocket-dial) · C++17 SIP registrar + PBX for ESP32-S3 and desktop. Point any SIP phone at it and start calling.
- [pocket-dial-handset](https://github.com/GlomarGadaffi/pocket-dial-handset) · ESP32-S3 SIP handset: push-to-talk G.711 over Wi-Fi, registers to pocket-dial.
- [resiprocate](https://github.com/GlomarGadaffi/resiprocate) · vendored reSIProcate: SIP / ICE / TURN / STUN / RTP stack.

### Wi-Fi / BLE
- [wifi-ble-marauder](https://github.com/GlomarGadaffi/wifi-ble-marauder) · ESP-IDF Wi-Fi/BLE security tool: 5 GHz deauth, Thread/Matter/Zigbee, BLE 5 extended adv. No Arduino.
- [deauth-detector](https://github.com/GlomarGadaffi/deauth-detector) · distributed 802.11 attack detector with a LoRa back-haul.
- [wigle-wardriver](https://github.com/GlomarGadaffi/wigle-wardriver) · Wi-Fi/BLE wardriver for Wigle.net, GPS-tagged scans to SD.
- [esp32s3-mgmt-scanner](https://github.com/GlomarGadaffi/esp32s3-mgmt-scanner) · high-throughput passive 802.11 management-frame scanner for ESP32-S3.
- [ble-sign-beacon](https://github.com/GlomarGadaffi/ble-sign-beacon) · broadcast a short message as a BLE advertisement. Deliberately visible, not hidden.

### LoRa / RF
- [lora-rf-toolkit](https://github.com/GlomarGadaffi/lora-rf-toolkit) · LoRa RF reverse-engineering: sweep, I/Q capture, chirp and parameter analysis on SX1262.
- [fsk-walkie-talkie](https://github.com/GlomarGadaffi/fsk-walkie-talkie) · voice-over-FSK walkie-talkie (Codec2 + SX1262).

### Scanner (Uniden BCD325P2)
- [bcd325p2-protocol](https://github.com/GlomarGadaffi/bcd325p2-protocol) · serial command-protocol reference for the BCD325P2.
- [bcd325-splunk-addon](https://github.com/GlomarGadaffi/bcd325-splunk-addon) · Splunk add-on: ingest serial RF telemetry, parse P25/EDACS, emit indexed JSON.
- [bcd325-dashboard](https://github.com/GlomarGadaffi/bcd325-dashboard) · decode, visualize, and persist BCD325P2 telemetry (archive + real-time modes).
- [p25-trunk-logger](https://github.com/GlomarGadaffi/p25-trunk-logger) · P25 trunked-radio control-channel logger; builds trunk-recorder configs from RadioReference.

### Mesh / radio networking
- [meshtap](https://github.com/GlomarGadaffi/meshtap) · passive Meshtastic capture to BigQuery over cellular MQTT.
- [reticulum](https://github.com/GlomarGadaffi/reticulum) · vendored Reticulum: cryptography-based mesh networking over LoRa, packet radio, serial, TCP.
- [rfparty](https://github.com/GlomarGadaffi/rfparty) · vendored rfparty: wireless situational-awareness dashboard for BLE/Wi-Fi telemetry.

### Comms / crypto
- [tor-voice](https://github.com/GlomarGadaffi/tor-voice) · encrypted voice over Tor: in-process Arti onion service + Opus + Noise, no daemons.
- [glossh](https://github.com/GlomarGadaffi/glossh) · minimal SSH 2.0 server for ESP-IDF on PSA Crypto (curve25519 / aes256-gcm / ecdsa-p256).
- [esp-secure-transport](https://github.com/GlomarGadaffi/esp-secure-transport) · MIT/PD secure-transport stack for ESP-IDF. Paused in favor of glossh; kept for reference.

### Hardware / tooling
- [jc3248-display-driver](https://github.com/GlomarGadaffi/jc3248-display-driver) · ESP-IDF driver + bring-up for the Guition JC3248W535EN (ESP32-S3, AXS15231B QSPI 320x480).

### Agents / data
- [esp32-ai-agent](https://github.com/GlomarGadaffi/esp32-ai-agent) · ESP32 AI agent with persistent memory and an offline rule engine; configure over Telegram / serial / NATS.
- [ask-the-logs](https://github.com/GlomarGadaffi/ask-the-logs) · natural-language queries over BigQuery via Google ADK + Gemini.

### Synthetic demos
- [deanon-demo](https://github.com/GlomarGadaffi/deanon-demo) · what ~$900 of commodity hardware can reconstruct about multi-channel pseudonymity. Synthetic data only.
- [sentinel-node-demo](https://github.com/GlomarGadaffi/sentinel-node-demo) · synthetic demo of second- and third-order surveillance / counter-surveillance effects. Synthetic data only.

### Other
- [rdp-publisher-cert](https://github.com/GlomarGadaffi/rdp-publisher-cert) · provisions a publisher certificate for .rdp files: self-signed cert, Group Policy, consent-prompt bypass.
