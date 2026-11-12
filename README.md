# Parcel Tracker API (demo)

A small fictional API specification. It exists to demonstrate
[Truthpage for Confluence](https://gist.github.com/aminredfield/381092b3d811b6acbbe6012d134aac16):
a Confluence page documents these endpoints, and Truthpage checks the page against `openapi.yaml`
at an exact commit, re-checking it on every push.

Nothing here is a real service. The file `openapi.yaml` is the only source of truth.

## Endpoints

| Method and path | Purpose |
|---|---|
| `GET /parcels` | List parcels, filtered by `status`, limited by `limit` |
| `POST /parcels` | Register a parcel |
| `GET /parcels/{id}` | Read one parcel |
| `GET /parcels/{id}/events` | Tracking events of a parcel |
| `GET /couriers/{id}` | The courier assigned to deliveries |
| `PATCH /notifications/settings` | Choose which events send a notification |

## Licence

MIT, see `LICENSE`.
