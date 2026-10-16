# Architecture notes

The browser app is a static prototype. `OG_STORE` is the only persistence layer and stores data in the current browser's localStorage. This means data is per-browser/device and can be cleared by the user. A real cross-device account needs a backend and authentication.

`OG_MATCHMAKING` only displays a simulated lobby. It does not discover real players or connect clients. `OG_MATCH` is a local reward simulator; production rewards must be validated by a trusted server to prevent cheating.
