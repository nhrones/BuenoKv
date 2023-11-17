# BuenoKv
![Alt text](Bueno.jpg)   

BuenoKv is a key/value database that uses the same semantics and serialization as DenoKv.    
The intent is to provide data that is both compatible with, and transferable to and from DenoKv.

## Goals
- Mirror most of the Deno.Kv API 
- Support ACID-transactions for Key-Value CRUD using any persistence service
  - Include transaction-wrapped basic RPC services for remote persistence
- Implement serialization (codecs) for multipart-keys and values
  - See:  https://nhrones.github.io/kv-key-codec/ 
- Provide a consistent cache-service for typed collections (BuenoCache)
  - High performance data presentation and consistent mutations
  - Instant filtering, ordering, pagination
  - Full text search per column (property)
    - See: https://nhrones.github.io/BuenoCache/
- Require no external dependencies (Deno not required)
  - Provided library and tools to be browser compatible

