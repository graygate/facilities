# graygate facilities

Hospitals, pharmacies and drinking water, cut into 1° tiles, for the graygate app's offline
"nearby places" list. The app fetches only the tiles around the phone.

- `facilities/index.json` — signed index (Ed25519, the graygate manifest key), one entry per country
- `facilities/<CC>/tiles.json` — the country's tiles, trusted by the hash in the signed index
- `facilities/<CC>/<lat>_<lng>.json` — one tile's places, trusted by the hash in the tile list

Data © OpenStreetMap contributors, available under the Open Database License (ODbL 1.0):
https://www.openstreetmap.org/copyright
