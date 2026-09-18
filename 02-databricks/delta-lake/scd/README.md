# SCD — Slowly Changing Dimensions

- scd1.py — Type 1: overwrites the changed row; no history kept.
- scd2.py — Type 2: closes the old version (end_dt, isActive=N) and inserts a new version (start_dt, isActive=Y); full history.

Key columns for SCD2: start_dt, end_dt, isActive. Change detection via row hashkey.
