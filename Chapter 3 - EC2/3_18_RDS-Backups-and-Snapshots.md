#### Two ways to backup RDS

### Database Snapshots

- Manual, and user initiated.

- No retention period.

- You might use this when planning to make massive changes to a database. Right before making the changes (rather than waiting for automatic backups), initiate a snapshot, and get to work.

### Automated Backups

- Enabled by default, creating daily backups or snapshots during a window of time specified by the user.
  - Free storage space == database size.

1. Allows you to recover a database to any point within a retention period of 1-35 days.
2. Full Daily backups, and also provides transaction logs throughout the day.
3. Recovery Process - when recoverying, AWS will select the most recent backup and restore what was found in the transaction logs.

- Snapshots stored in S3.

### Encryption at Rest

- Enable this at time of creation by selecting "Encryption" in the creation console.
- Completely integrates with KMS.
- Includes all underlying storage, automated backups, snapshots, and read replicas.

_You cannot enable encryption on an initially unencrypted database._ What you can do is take a snapshot encrypt the snapshot, perform a database restore with the encrypted snapshot. Try to avoid this at all costs, but the option to do this is there if a database that isn't encrypted suddenly needs to be.
