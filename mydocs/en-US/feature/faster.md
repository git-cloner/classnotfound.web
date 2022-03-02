---
name: Faster
---

# Faster

Synchronizing the data from maven central, the class info is parsed and saved locally, search speed is up to milliseconds.

Jar data and classname and jar correspondence, stored in the mysql database, due to fewer fields, Java class names generally do not use full-text search, as long as the establishment of a suitable index, directly according to the SQL query can obtain a higher query speed.

