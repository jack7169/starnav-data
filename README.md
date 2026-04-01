# starnav-data

Automated data cache for [StarNav](https://github.com/jack7169/Starnav). Updated by GitHub Actions.

## Data

| File | Source | Frequency | Description |
|------|--------|-----------|-------------|
| `tle/starlink.json` | CelesTrak | Every 2h | Starlink constellation TLE data |
| `geoid/egm96_15min.json` | NGA EGM96 | Static | Geoid undulation grid (15' resolution) |

## Usage

StarNav fetches data from `raw.githubusercontent.com` URLs:

```
https://raw.githubusercontent.com/jack7169/starnav-data/main/tle/starlink.json
```

This avoids CelesTrak rate limits (2h) and CORS restrictions.
