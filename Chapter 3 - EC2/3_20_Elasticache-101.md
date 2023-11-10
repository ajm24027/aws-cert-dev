### What is Elasticache

Elasticache is an in-memory cache. It stores frequently accessed data to increase Database performance by delivering data faster than retrieving data from a disk.

- Good for storing session data for distributed applications.

Database > Elasticache > App (Faster)

Database >>>>>>>>>>>>>>> App (Slower)

#### 2 Types of ElastiCache

1. MemChaced

- Great for basic object caching, scales horizontally, but there is no persistence, multi-AZ, or failover.

- Good for when you just want basic caching.

2. Redis

- Includes everything Memcached Doesn't.

- Supports sorting and ranking data (e.g. gaming leaderboards) and complex datalists like lists, and hashes.
