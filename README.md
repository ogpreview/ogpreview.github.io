# ogpreview.github.io
Preview Open Graph / Twitter Card metadata for any URL. No API key needed.

## Changelog

The current version is shown at the bottom of the page.

Link to a preview directly with `https://ogpreview.github.io/url/<url-encoded link>` (same format as opengraph.xyz) or `?url=<link>`.

- **4.0.0** (2026-10-28): Minimal monospace redesign (JetBrains Mono, stone palette, flat cards) from the design handoff; checks summary and fallback info; over-limit notes on fields; outline tag chips; Download all PNGs now saves one zip.
- **3.1.0** (2026-10-28): Desktop / Mobile preview switch with phone frames and mobile layouts; per-platform list of the tags each one reads (found / missing); download any preview as PNG, or all at once. The Worker now also passes images through so they appear in PNGs (redeploy it).
- **3.0.0** (2026-10-28): opengraph.xyz-style UI: previews for Google, Facebook, X, LinkedIn, Discord, Slack and WhatsApp; editable metadata with live previews; checks for missing/long tags and image size; generated meta tags to copy; shareable `/url/<encoded-url>` links.
- **2.2.0** (2026-10-28): Use our own Cloudflare Worker proxy (`ogpreview.iniret.workers.dev`) first; public proxies are now only a fallback.
- **2.1.0** (2026-10-28): Query all proxies in parallel and use the fastest; shorter timeout; optional own proxy (`CUSTOM_PROXY`, see `worker/README.md`).
- **2.0.0** (2026-10-28): Fetch OG data without an API key (CORS proxies + Microlink fallback), link-card preview, full tag table, copy as JSON, shareable `?url=` links, version footer.
- **1.0.0**: Initial version using opengraph.io.
