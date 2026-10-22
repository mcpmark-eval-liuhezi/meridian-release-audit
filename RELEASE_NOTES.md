# Meridian Release Notes

## Release 2.4.0

### Changes
- Fixed telemetry buffer overflow on restart
- Upgraded metrics SDK to 3.9.2
- Added retry backoff for webhook delivery (ref #412)

### Known issues
- Nightly export still skips empty partitions
