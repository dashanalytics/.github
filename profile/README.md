![](https://dashanalytics.pages.dev/assets/dashanalytics-D05VPhbo.svg)
# Introduction
**Quickly deploy your analytics service on your machine. Just build and run!**

The original intention of doing this was that I couldn't find any analysis server software that could run on `riscv64` target.
So I wrote `analytics-server` in Go that only depends on the standard library and Redis.

## Self-host

Working with [Redis](https://redis.io/learn/howtos/quick-start).
Simple and flexable.

NOTE: Source IP and country recording is not available without support from cloud service provider.

## Behind your reverse proxy provider.

**Dashanalytics** also provided for hosts behind a reverse proxy.
Get specific client information from specific HTTP headers.
Such as source IP and country.

For example, Cloudflare: specify the header `CF-Connecting-IP` and `CF-IPCountry` so that the server will recognize and record them.
