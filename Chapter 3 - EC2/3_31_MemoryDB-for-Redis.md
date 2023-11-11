### MemoryDB for Redis

In-Memory Databse, has Multi-AZ, and can be used as a primary database. Can support 160,000,000req/s. Offers microsecond read and write latency.

#### Use Case

Great for Redis-Compatible Databases.

- Online Gaming company needs a way for millions of concurrent users, rendering 3d worlds with assets.

#### Elasticache vs MemoryDB

1. Elasticache is a database cache service that sits infront of a database. Used for websites to store session data.
2. MemoryDB can be used as a primary database, ultrafast performance. Would be good for that massive online gaming company.

#### Exam Tips

1. MemoryDB is an ultrafast In-Memory DB with Microsecond read and single digit millisecond write.
2. Highly performant, large-scale microservice applications (online gaming company sharing assets to millions of users).
3. MemoryDB can store an entire dataset in memory, no DB required vs. Elasticache is an in-memory cache for databases. Cache vs in-memory dataset or database.
