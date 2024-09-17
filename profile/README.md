## Fastly deploy analytics service

### Self-hostable

Build and run.
Working with [Redis](https://redis.io/learn/howtos/quick-start).
Simple and flexable.

NOTE: Source IP and country recording is not available without support from cloud service provider.

### Behind your reverse proxy provider.

**Dashanalytics** also provided for hosts behind a reverse proxy.
Get specific client information from specific HTTP headers.
Such as source IP and country.

For example, Cloudflare: specify the header `CF-Connecting-IP` and `CF-IPCountry` so that the server will recognize and record them.
