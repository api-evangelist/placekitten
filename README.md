# PlaceKitten (placekitten)

Placeholder kitten image service. A community staple from the 2010s used alongside `placehold.it` for design comps, prototype layouts, and demos.

**APIs.yml:** [apis.yml](apis.yml)

## Status: DEPRECATED

As of **2026-05-30**, `https://placekitten.com/` (and `/{width}/{height}`, `/g/{width}/{height}`) returns **Cloudflare HTTP 521** ("Web server is down"). DNS still resolves to Cloudflare edge IPs, but the origin is unreachable. Treat the service as defunct.

**Recommended alternatives:** [picsum.photos](https://picsum.photos), [placedog.net](https://placedog.net), [place-hold.it](https://place-hold.it), or self-hosted assets.

## Type
- **x-type:** opensource (community placeholder service)
- **x-tier:** 3 (bulk-registered from public-apis)
- **x-status:** deprecated
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Animals

## URL Contract (historical)
| Path | Description |
|---|---|
| `/{width}/{height}` | Color kitten JPEG at requested size |
| `/g/{width}/{height}` | Grayscale kitten JPEG at requested size |

Example: `https://placekitten.com/200/300`, `https://placekitten.com/g/400/600`

## Artifacts

| Artifact | Path |
|---|---|
| OpenAPI 3.0 spec | [`openapi/placekitten-openapi.yml`](openapi/placekitten-openapi.yml) |
| JSON Schema — request | [`json-schema/placekitten-image-request-schema.json`](json-schema/placekitten-image-request-schema.json) |
| JSON Schema — response | [`json-schema/placekitten-image-response-schema.json`](json-schema/placekitten-image-response-schema.json) |
| JSON Structure | [`json-structure/placekitten-image-request-structure.json`](json-structure/placekitten-image-request-structure.json) |
| JSON-LD context | [`json-ld/placekitten-context.jsonld`](json-ld/placekitten-context.jsonld) |
| Spectral ruleset | [`rules/placekitten-rules.yml`](rules/placekitten-rules.yml) |
| Shared capability | [`capabilities/shared/placekitten.yaml`](capabilities/shared/placekitten.yaml) |
| Workflow capability | [`capabilities/fetch-placeholder-image.yaml`](capabilities/fetch-placeholder-image.yaml) |
| Vocabulary | [`vocabulary/placekitten-vocabulary.yml`](vocabulary/placekitten-vocabulary.yml) |
| Examples | [`examples/`](examples) (3 files) |

## Tags
Animals, Public APIs, Placeholder, Images, Deprecated

## Notes
- Original author: **Mark James** (http://mark.james.name), inspired by `placehold.it`.
- There is no canonical PlaceKitten GitHub organization or first-party SDK; the GitHub ecosystem only contains third-party language wrappers (Ruby, Django, jQuery, Angular, Swift, PHP, Python, etc.).
- Free, no authentication, no documented rate limits — pricing/rate-limits/finops profiling intentionally skipped per opensource defunct-service pipeline.
- Original entry bulk-registered as part of a public-apis catalog sweep on 2026-05-28; full enrichment pipeline run on 2026-05-30 confirmed defunct status.

## Timestamps
- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## Maintainers
- **Kin Lane** — kin@apievangelist.com
