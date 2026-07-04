# mbt-SiT5721-lib

Shared Python library for talking to the SiT5721 GPSDO over I2C
(`SiT5721` class in `mbt_SiT5721_lib.py`). Used by both:

- `mbt-ubx-apps` (GNSS calibration capture) - `get-data.py`, `check-SiT5721-defaults.py`
- `SiT5721` (GPSDO restart/save tooling) - `read-SiT5721.py`, `restart-SiT5721.py`, `save-SiT5721.py`

Consumed as a git submodule at `lib/mbt-SiT5721-lib` in both repos.

## History

Split out on 2026-07-04 from what had been two independently git-tracked,
manually-synced copies of this file (one in each consuming repo). The
commit history above is the real history of the file, reconstructed from
both repos' logs: it was created in `mbt-ubx-apps` (`a40590b`, `ff31166`),
copied into a new `SiT5721` repo which then carried it forward
(`23df980` = a duplicate of `ff31166`'s content, `d4e7b07`, `8a2018f`),
then synced back into `mbt-ubx-apps` (`ff2976f` = a duplicate of
`8a2018f`'s content). The two duplicate sync commits were dropped here;
everything else is preserved with its original author, date, and message.
