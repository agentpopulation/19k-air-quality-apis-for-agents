## Air quality API endpoints, snapshot 15 Nov 2026

- 19,833 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 1,268 services · 247 country codes · 9,833 keyless JSON rows

### Download

- `Air_Quality_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 19,833 rows, 931.8 kB gzipped (6.7 MB as CSV), SHA-256 `d719067d28933c072c419336066d8591c72f3a1f9c5cacfe7d3a88bdc3f577bb`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Air_Quality_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Air_Quality_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 7,630 · Wrap one URL pattern as a get_air_quality tool: pass a latitude and longitude or a station series id, return PM2.5, PM10, ozone and NO2 with the time of the reading.
- 📱 App features: 3,971 · Show PM2.5, PM10 and US AQI for a city on a card, and draw monitoring sites, pollution zones or modelled annual means as a map layer.
- 🧠 Grounding and data pipelines: 10,260 · Load station series and country PM2.5 figures on a schedule into your own store, so answers about air pollution cite a dated source.
- 🧪 Evals and testing: 19,833 · Run your air-quality tool against a fixed set of URLs across formats; check that pollutant, unit, value and timestamp parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release: 20,830 endpoints from 1,511 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 19,833 endpoints from 1,268 services, 997 fewer endpoints than first published under this snapshot (20,830 from 1,511 services), tested 10–15 Nov 2026 (IST).
- Left out: 157 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 layer marked editable in the title (it can hold entries that people added).
- Left out: 20 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 293 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 11 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 16 ArcGIS layers that are records about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 9 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 327 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 76 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 470 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 78 rows that repeat an address already in the pack.
- Overlap: 19,829 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 6,101 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 319 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 16 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 11 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 363 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 20 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 24 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 122 of these URLs are also in 22k-maritime-apis-for-agents.
- Overlap: 11,535 of these URLs are also in 160k-environment-apis-for-agents.
- Overlap: 560 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 9,831 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 183 of these URLs are also in 84k-health-apis-for-agents.
- Overlap: 86 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 48 of these URLs are also in 40k-hazards-apis-for-agents.
- Overlap: 13 of these URLs are also in 4.9k-wildfire-apis-for-agents.
- Overlap: 115 of these URLs are also in 67k-energy-apis-for-agents.
- Overlap: 13 of these URLs are also in 23k-aviation-apis-for-agents.
- Overlap: 30 of these URLs are also in 22k-traffic-apis-for-agents.
- Overlap: 1 of these URLs is also in 10k-parking-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Air quality API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
