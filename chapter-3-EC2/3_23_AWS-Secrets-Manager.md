### AWS Secrets Manager

Exactly like what we were doing at Heroku and what we were trying to do with the calendar app - Storing the .env variables in a secure location, but the app still having access to it.

Store Username & Passwords, Server Addresses, DB Name & Port - for use with Databases.

- Secrets can be rotated automatically every 30, 60, 90, or a custom amount of days.

### Secrets Manager vs Parameter Store:

1. Secrets Manager - Database Creds, API Keys, Rotation of Keys.
2. Parameter Store - Wider Use Cases, Configuration Variables, License Keys.

### Exam Tips

Centrally Manage Secrets and rotate them.

RDS Database, Redshift Cluster, DocumentDB Database, and API Keys can be integrated with Secrets Manager. 

