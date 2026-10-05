# 7-Day Kenya Safari Route Map: Masai Mara, Lake Nakuru, Lake Naivasha & Amboseli
 
An interactive 3D map of a 7-day road safari across Kenya's classic circuit. The trip starts and ends at **Jomo Kenyatta International Airport** in Nairobi. Along the way it crosses the Great Rift Valley to the **Masai Mara**, visits the flamingo lake of **Lake Nakuru** and the freshwater **Lake Naivasha**, and finishes in **Amboseli** beneath Kilimanjaro.
 
🗺️ **See the full itinerary and the live map:**
[7-dniowe safari w Kenii – prawdziwa przygoda](https://safarikenia.com.pl/7-dniowe-safari-w-kenii-prawdziwa-przygoda) on **Safari Kenia**
 
---
 
## The route
 
| Day | Destination | Accommodation |
|-----|-------------|---------------|
| Start | Arrival in Nairobi | Jomo Kenyatta International Airport |
| Day 1 | Masai Mara National Reserve | Mara Sopa Lodge |
| Day 2 | Talek region, Masai Mara | Talek |
| Day 3 | Lake Nakuru National Park | Lake Nakuru Sopa Lodge |
| Day 4 | Lake Naivasha | Lake Naivasha Sopa Resort |
| Day 5 | Amboseli National Park | Amboseli Sopa Lodge |
| Day 6 | Exploring Amboseli | Amboseli National Park |
| Day 7 | Departure | Jomo Kenyatta International Airport |
 
**Into the Mara:** Nairobi → Mai Mahiu (Rift Valley escarpment) → Narok → Masai Mara
**Rift Valley lakes:** Mara → Narok → Naivasha → Lake Nakuru → Gilgil → Lake Naivasha
**South to Kilimanjaro:** Naivasha → Nairobi → Kajiado → Amboseli
**Back to Nairobi:** Amboseli → Namanga → Athi River → JKIA
 
The interface labels are in Polish, matching the tour page it's embedded on.
 
## Features
 
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain (1.5× exaggeration) and a tilted camera. This shows the drop into the Great Rift Valley and the lakes on its floor.
- **Road-accurate route.** All 17 legs come from the Mapbox Directions API (driving profile) and are stitched into one continuous line. If a request fails, the map falls back to a straight segment for that leg.
- **Glowing animated route line.** The route is drawn as a golden "marching ants" line with emissive strength, so it stays bright over the satellite imagery.
- **Interactive itinerary panel.** A glassmorphism sidebar lists all seven days. Clicking a card flies the camera to that stop.
- **Waypoint-guided routing.** Hidden waypoints keep the line on the real roads: Mai Mahiu, Narok, Gilgil, Kajiado, Namanga and others.
- **Mobile-friendly.** On small screens the sidebar becomes a bottom sheet, and cooperative gestures keep page scrolling smooth.
- **WordPress-ready.** Styles are scoped to a single container, so the code can be pasted into a Custom HTML block.
## Tech stack
 
- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, with no build step
- Plus Jakarta Sans (Google Fonts)
## Usage
 
1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.
To change the route, edit the `itineraryData` array. Entries with `isWaypoint: true` shape the route only. All other entries get a marker and a sidebar card.
 
## About
 
Built for [Safari Kenia](https://safarikenia.com.pl/), Polish-language safari tours and travel guides for Kenya.
 
➡️ [View this 7-day Kenya safari itinerary](https://safarikenia.com.pl/7-dniowe-safari-w-kenii-prawdziwa-przygoda)
