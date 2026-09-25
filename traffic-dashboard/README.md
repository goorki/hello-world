# Gantry G-07 Flow Desk

A single-file decision support dashboard for data from a tolling gantry. Each record is one crossing:
`timestamp, lane, vehicle_type, speed, license_plate, headway`.

Open `index.html` in a browser. It loads a simulated weekday (about 53,000 crossings, 3 lanes). Use **Load CSV** to analyse your own file.

## What it shows

**Decision support (all lanes, all classes, last 15 min)**
- Traffic state and HCM level of service from density in pc/km/ln (k = q / space-mean speed).
- Rule engine on 5-minute aggregates: queue at the gantry, lane blockage, breakdown risk (flow vs. the 97th-percentile capacity), short headways (< 1 s), speeding (> limit + 20 km/h), HGVs in the left lane, low ANPR read rate.
- Proposed VMS message, lane control signals and a full-day alert timeline.

**Transport economics**
- AC and MSC curves from the fitted speed–density model, linear inverse demand with a chosen elasticity.
- Optimal Pigouvian charge τ* where P(q) = MSC(q), optimal flow, welfare gain, and a surcharge or off-peak discount relative to the flat tariff. Flags hypercongested states where a bottleneck (Vickrey) model applies.

**Traffic flow theory (filterable by lane and class)**
- Flow and space-mean speed per lane, lane × time speed contour.
- Fundamental diagrams (v–k, q–k, v–q) with Greenshields, Underwood and Drake fits and R².
- Time-headway distribution with negative and shifted exponential fits and KS statistics.
- Spot-speed distribution by class with v15/v50/v85 and the 10 km/h pace.
- Lane use and fleet mix, toll revenue and PCE by class.
- Speed violations (masked plates), frequent crossers, data quality (duplicates, implausible values, plate read rate).

## Sample scenario

Stochastic breakdown in the morning peak with a 10% capacity drop, lane 1 blocked 12:50–13:25, night-time speeding, short headways in the evening peak, HGVs overtaking 10:05–11:05, and a dirty ANPR lens on lane 2 after 20:00.
