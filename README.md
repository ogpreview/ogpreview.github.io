# ogpreview.github.io
Preview Open Graph / Twitter Card metadata for any URL. No API key needed.

## Changelog

The current version is shown at the bottom of the page.

- **2.2.0** (2026-10-28): Use our own Cloudflare Worker proxy (`ogpreview.iniret.workers.dev`) first; public proxies are now only a fallback.
- **2.1.0** (2026-10-28): Query all proxies in parallel and use the fastest; shorter timeout; optional own proxy (`CUSTOM_PROXY`, see `worker/README.md`).
- **2.0.0** (2026-10-28): Fetch OG data without an API key (CORS proxies + Microlink fallback), link-card preview, full tag table, copy as JSON, shareable `?url=` links, version footer.
- **1.0.0**: Initial version using opengraph.io.
