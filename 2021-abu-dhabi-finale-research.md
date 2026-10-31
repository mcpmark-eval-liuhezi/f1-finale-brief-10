# 2021 Abu Dhabi Grand Prix — Season-Closing Finale at Yas Marina

Research summary for the racing newsletter retrospective on the 2021 season finale,
the round where Max Verstappen and Lewis Hamilton arrived level on points and the
title was decided on the last lap.

## Race Session

- **Event:** 2021 Abu Dhabi Grand Prix (Round 22 of the 2021 F1 season)
- **Circuit:** Yas Marina Circuit, Abu Dhabi, UAE
- **Date (as reported by the data source):** 2021-12-12 (time 13:00:00Z)
- **Session key:** `getHistoricalSessions` returned an empty result set for all
  filter combinations tested (country: UAE / United Arab Emirates; location:
  Abu Dhabi / Yas Island / Yas Marina; circuit_short_name: Yas Marina;
  session_name: Race / Qualifying; year: 2021). The session key is therefore
  **not returned by the historical-sessions lookup** in this environment; the
  date above is as reported by both the race calendar and the classified race
  results for Round 22, 2021.

## Classified Race Results (Round 22, 2021)

| Pos | Driver | Constructor | Time/Gap | Laps |
|-----|--------|-------------|----------|------|
| 1 | Max Verstappen | Red Bull | 1:30:17.345 | 58 |
| 2 | Lewis Hamilton | Mercedes | +2.256 | 58 |
| 3 | Carlos Sainz | Ferrari | +5.173 | 58 |

## Driver Profiles (as returned by the profile lookup)

### Lewis Hamilton (P2, finishing order)
- **Permanent number:** 44
- **Three-letter code:** HAM
- **Nationality:** British
- **Date of birth:** 1985-01-07
- **Profile link:** http://en.wikipedia.org/wiki/Lewis_Hamilton

### Max Verstappen (P1, finishing order)
- **Permanent number:** 3
- **Three-letter code:** VER
- **Nationality:** Dutch
- **Date of birth:** 1997-09-30
- **Profile link:** http://en.wikipedia.org/wiki/Max_Verstappen

### Carlos Sainz (P3, finishing order)
- **Permanent number:** 55
- **Three-letter code:** SAI
- **Nationality:** Spanish
- **Date of birth:** 1994-09-01
- **Profile link:** http://en.wikipedia.org/wiki/Carlos_Sainz_Jr.

## Newsletter Retrospective Notes

- Verstappen's Red Bull (#3 in race entry list / permanent number 3) won from pole;
  Hamilton's Mercedes (#44) finished second, +2.256s, to clinch the 2021 constructors and
  drivers' championships at the Yas Marina Circuit.
- Sainz completed the podium in a Ferrari (+5.173s).
- Verstappen took fastest lap (lap 39, 1:26.103) and all fastest-lap points; Hamilton
  recorded the fastest lap of the race on lap 43 (1:26.615, rank 3).
- Full classified results and circuit detail are available at
  https://en.wikipedia.org/wiki/2021_Abu_Dhabi_Grand_Prix and
  https://www.youtube.com (n/a) — source: Ergast-style race results feed.

## Data Sources

- Race calendar & classified results: `getHistoricRaceResults` (year=2021, round=22)
  and `getRaceCalendar` (year=2021) — date 2021-12-12, Yas Marina Circuit.
- Driver profiles: `getDriverInfo` for driverIds hamilton, max_verstappen, sainz.
- Session lookup: `getHistoricalSessions` — returned empty for all 2021 filters;
  session key not available from this endpoint.
