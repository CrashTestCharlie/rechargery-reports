# Ionna Locations Reports

A weekly snapshot of [IONNA] EV charging station locations across the US
— where they are, what kind they are, and whether they’re open yet.

The raw data is scraped from IONNA’s website every Sunday night. Each
week’s snapshot lands in two folders:

- **`data/`** — the raw HTML page as it was scraped, kept as-is for the
  record.
- **`reports/`** — a human-friendly summary report (`.md`) and the
  extracted location data (`.json`).

## What’s in a report

Each report starts with the total location count and the date the data
was gathered, followed by four tables:

### Locations by State

A count of locations in each state, so you can see at a glance where
IONNA has built out the most (and where they haven’t shown up yet).

### Locations by Type

A count of locations by the kind of site, using IONNA’s own names:

**Rechargery** (their standalone charging sites)  
**Rechargery \@** (sites hosted at a partner business — a Wawa, Sheetz,
Casey’s, etc.)  
**Relay** (sites with chargers, near facilities)  
**Beacon** (undescribed)

### Locations by Status

The full list of every location, grouped by status — **Open**, **Opening
Soon**, or **Under Renovation** — and sorted by state. This is the table
to skim if you want to spot what’s newly open or coming to your area.

### Locations by Speed

A count of locations by their maximum charging speed. (So far, they’re
all 400 kW.)

  [IONNA]: https://www.ionna.com/
