# Discovery catalogue

Generated 2026-11-12 from the Jobscout API (active listings only). All pages were paginated to exhaustion (`next_before_id` cursor; no page left unfetched).

## Title queries (all paginated, deduplicated by job ID)

| Query | Active matches |
| :--- | ---: |
| video editor | 791 |
| video cutter | 17 |
| cutter | 330 |
| videographer | 173 |
| video producer | 275 |
| motion graphics | 146 |
| film editor | 2 |
| video post-production | 3 |
| content editor video | 48 |

1,661 unique listings after merging. 313 were then excluded as non-video false positives (meat/die/wire/pattern cutters, machinists, tailors and similar from the broad `cutter` query). 225 listings remained for screening: 19 Berlin, 79 USA remote, 127 Europe remote (5 Berlin remote roles appear on both Berlin and Europe pages).

## Screening rules

- Berlin: `location_city` Berlin or location text contains Berlin.
- USA: country United States and `work_arrangement` remote.
- Europe: `work_arrangement` remote and (European country, or geographic scope europe/emea/eu/worldwide/global, or location text like "Remote Europe"). LatAm-only and Southeast-Asia-only remote listings excluded.
- "Discovery candidates" are everything above; no eligibility claims beyond what each Jobscout record states. Residency, travel and scope notes are shown per row where the record supplies them.
- Jobgether rows are anonymized "partner company" listings in the source itself; the hiring employer is not named in the API data.
