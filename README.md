# polytrace

A simple web tool to visualize encoded polyline routes (from OSRM or similar sources) on a map using Leaflet and OpenStreetMap.

## Features

- Paste raw JSON from OSRM
- Decodes `geometry` into route line on map
- Adds start and end markers with latitude/longitude
- Uses Leaflet + OpenStreetMap (no API keys required)
- Ready for GitHub Pages deployment

## Demo

[Live Demo on GitHub Pages](https://anggaprytn.github.io/osrm-route-viewer/)

## How to Use

1. Open the website.
2. Paste your JSON data containing a `geometry` and `waypoints` field.
3. Click **Render Route**.
4. See the polyline drawn and markers shown for start/end points.

## Deployment

To deploy on GitHub Pages:

1. Clone this repo
2. Push your changes to the `main` branch
3. Go to repository Settings → Pages → Source → `main` → root
4. Save and visit the provided URL

## Example JSON format

```json
{
  "routes": [
    {
      "geometry": "your_encoded_polyline"
    }
  ],
  "waypoints": [
    { "location": [lng, lat] },
    { "location": [lng, lat] }
  ]
}
