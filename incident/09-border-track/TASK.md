# Task 9 — Border track

`track.ewlog` is the navigation log from a hostile drone brought down by jamming in the Barmer sector of India's western international border. Positions are metres from a reference point, not latitude and longitude.

The flag uses checksum-valid records only. Takeoff is the earliest valid telemetry fix. Landing is the latest valid telemetry fix. Waypoints are the valid route records, in sequence order.

Submit that flag in this shape and no other. The numbers below are an example of the characters, not the drone's position:

```
Intern_Pro_Max{TO:12.34567,98.76543|W:12.00000,98.00000;12.10000,98.10000|LD:12.50000,99.00000}
```

- Three parts, in this order, separated by `|`: `TO:`, then `W:`, then `LD:`.
- `TO:` is the takeoff latitude, a comma, the takeoff longitude.
- `W:` is every waypoint as `latitude,longitude`, separated by `;`, in sequence order. No `;` after the last waypoint.
- `LD:` is the landing latitude, a comma, the landing longitude.
- Latitude first, longitude second.
- Exactly 5 digits after each decimal point, including trailing zeros.
- Round using the next digit: 0 to 4 leaves the last digit, 5 to 9 increases it.
- A negative coordinate keeps its minus sign. Do not write a plus sign.
- No spaces. No `N`, `E`, `S`, `W` hemisphere letters. No degree symbol.

Once a record is in metres east and north of the reference point:

```
latitude = ref_lat + north_m / 111320
longitude = ref_lon + east_m / (111320 * cos(ref_lat in radians))
```
