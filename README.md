# polytrace

A simple web tool to visualize encoded polyline routes (from OSRM or similar sources) on a map using Leaflet and OpenStreetMap.

## Features

- Paste raw JSON from OSRM
- Decodes `geometry` into route line on map
- Adds start and end markers with latitude/longitude

## Demo

[Live Demo on GitHub Pages](https://anggaprytn.github.io/osrm-route-viewer/)

## How to Use

1. Open the website.
2. Paste your JSON data containing a `geometry` and `waypoints` field.
3. Click **Render Route**.
4. See the polyline drawn and markers shown for start/end points.

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
