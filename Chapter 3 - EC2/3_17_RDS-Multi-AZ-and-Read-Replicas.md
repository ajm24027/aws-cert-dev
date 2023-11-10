### What is Multi-AZ?

It is an exact copy of a production database in another availability zone.

- Primary RDS exists in us-east-1a, and a standby copy exists in us-east-1b. If us-east-1a goes down, RDS automatically fails over to the standby cloned RDS.

- When writing to a production database, the information is automatically cloned to this standby.

- A little like load balancer for RDS. But it's only for disaster recovery, Multi-AZ is not used to improve performance. This is what "read replicas" are for.

#### Read Replicas

- Not every part of a business will need read/write access to a DB. The app can have read/write access to the production RDS. But maybe the sales team only needs access to read the database, to write reports and such.

- Rather than everyone accessing and reading/writing from the production database, particular teams who only need to read, access the Read Replica.

- Automatic Backups need to be enabled for Read Replicas to clone the production database.
