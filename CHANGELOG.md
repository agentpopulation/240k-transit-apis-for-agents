# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- New snapshot: 271,658 endpoints from 14,930 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026; 165,931 more endpoints than the 14 Nov 2026 release (105,727 endpoints from 9,281 services).
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 249,684 endpoints from 14,126 services, 21,974 fewer endpoints than first published under this snapshot (271,658 from 14,930 services), tested 10–15 Nov 2026 (IST).
- The repository holds a 1,000-row sample and the services list; the full list is the release download Transit_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 240k-transit-apis-for-agents (was 270k-transit-apis-for-agents; first published as transit-api-endpoints). The name follows the count, rounded down.
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

## 2026-11-14 (snapshot-2026-11-14)

- First release: 105,727 endpoints from 9,281 services, tested 10–14 Nov 2026 (IST), snapshot 14 Nov 2026.
- The repository holds a 1,000-row sample and the services list; the full list is the release download Transit_API_Endpoints_AgentPopulation_Snapshot_2026-11-14.csv.gz.
- Left out: 77 rows whose URL carried a credential-looking parameter or a login.
- Left out: 1,458 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 35 rows whose title mentions trafficking (crime statistics tagged traffic, not transit).
- Left out: 3,033 rows whose subcategory mentions wetlands (map layers of wetlands, not transport).
