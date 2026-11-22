## Transit API endpoints, snapshot 15 Nov 2026

- 249,684 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 14,126 services · 249 country codes · 174,859 keyless JSON rows

### Download

- `Transit_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 249,684 rows, 11.0 MB gzipped (77.1 MB as CSV), SHA-256 `2c17e145694fc4821fc20e09c1687542243e3311230a884d57bce5bf93b5866f`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Transit_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Transit_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 16,074 · Wrap a GBFS station_status URL as a get_bike_availability tool: pass the system and station, return bikes and docks.
- 📱 App features: 30,018 · Show nearby parking and traffic counts on a map card.
- 🧠 Grounding and data pipelines: 38,416 · Load GTFS timetables and CSV tables on a schedule into your own store.
- 🧪 Evals and testing: 249,684 · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

### Changes

- New snapshot: 271,658 endpoints from 14,930 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026; 165,931 more endpoints than the 14 Nov 2026 release (105,727 endpoints from 9,281 services).
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 249,684 endpoints from 14,126 services, 21,974 fewer endpoints than first published under this snapshot (271,658 from 14,930 services), tested 10–15 Nov 2026 (IST).
- Left out: 4 rows whose URL carried a credential-looking parameter or a login.
- Left out: 18 rows with an email-like address.
- Left out: 2,800 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 2 ArcGIS proxy layers (utility.arcgis.com/usrsvcs and portal /sharing/servers/ addresses) that can call a service with a stored login.
- Left out: 31 layers marked editable in the title (they can hold entries that people added).
- Left out: 75 police traffic-stop layers (they can hold details of people stopped).
- Left out: 394 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 7,444 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 349 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 28 ArcGIS layers that are records about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 85 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Left out: 5 rows that are another address of an ArcGIS layer dropped for what it holds (one of the reasons above, found under another address of the layer).
- Left out: 367 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 7,370 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 1,175 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 14,557 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 154 rows that repeat an address already in the pack.
- Left out: 76 rows whose title mentions trafficking (crime statistics tagged traffic, not transit).
- Left out: 1,456 rows whose subcategory mentions wetlands (map layers of wetlands, not transport).
- Overlap: 8,804 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 2,469 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 2,580 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 404 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 22,597 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 605 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 1,381 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 1,836 of these URLs are also in 22k-maritime-apis-for-agents.
- Overlap: 502 of these URLs are also in 160k-environment-apis-for-agents.
- Overlap: 6,101 of these URLs are also in 19k-air-quality-apis-for-agents.
- Overlap: 4,865 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 174,255 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 278 of these URLs are also in 84k-health-apis-for-agents.
- Overlap: 134 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 345 of these URLs are also in 40k-hazards-apis-for-agents.
- Overlap: 14 of these URLs are also in 4.9k-wildfire-apis-for-agents.
- Overlap: 139 of these URLs are also in 67k-energy-apis-for-agents.
- Overlap: 1,179 of these URLs are also in 23k-aviation-apis-for-agents.
- Overlap: 22,790 of these URLs are also in 22k-traffic-apis-for-agents.
- Overlap: 10,779 of these URLs are also in 10k-parking-apis-for-agents.
- Overlap: 34 of these URLs are also in 7.8k-earthquake-apis-for-agents.
- Overlap: 64 of these URLs are also in 4.2k-volcano-tsunami-apis-for-agents.
- Overlap: 17,059 of these URLs are also in 17k-bike-share-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Transit API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
