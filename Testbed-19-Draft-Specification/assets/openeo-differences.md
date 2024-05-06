# Major differences with openEO

## Potentially Breaking Changes (for openEO clients)

- No support for well-known discovery (`/.well-known/openeo`)
- Header `OpenEO-Identifier` replaced with `GDC-Identifier`
- Use `gdc_version` instead of `api_version` in the landing page
- No support for STAC (API) 0.9

## Notable Changes (but clients should handle it fine)
- No budget / plan support
- No support for user-uploaded files (`/files`)
- No support for UDFs (`/udf_runtimes`)
- No support for OIDC (`/credentials/oidc`)
- Removal of `OpenEO-Costs` header

## Additions
- Addition of `/collections/{collection_id}/items` and `/collections/{collection_id}/items/...` (OGC API - Features and STAC API - Features, both version 1.0)
- Addition of `/collections/{collection_id}/coverages` and `/collections/{collection_id}/coverages/...` (OGC API - Coverages, version 0.0.2)