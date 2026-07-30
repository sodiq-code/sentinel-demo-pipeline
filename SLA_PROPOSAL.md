# SLA Proposal — raw_s3_nyc_taxi_trips

Asset: `urn:li:dataset:(urn:li:dataPlatform:s3,raw_s3_nyc_taxi_trips,PROD)`

## Proposed SLA

- **Type**: freshness
- **SLA seconds**: 3600 (1 hour)
- **Description**: The S3 landing zone must be modified at least every 1h.

## Rationale

The current incident fired when the dataset was 6h stale against a 1h SLA.
This file proposes tightening the assertion to a strict 1h SLA so the
next time the S3 ingestion job stalls, the alert fires earlier.

## Implementation

\\n
---
Proposed by Sentinel Agent (autonomous). NEVER merge without human review.
