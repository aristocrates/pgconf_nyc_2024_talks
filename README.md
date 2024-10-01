# Nick Meyer's PGConf NYC 2024 talks

## Testing your PostgreSQL backups (a practical guide)

Tuesday, 2024-10-01 11:40 UTC -4:00

https://postgresql.us/events/pgconfnyc2024/schedule/session/1735-testing-your-postgresql-backups-a-practical-guide/

It is often said that "an untested backup is not a backup" but how can we turn that saying into something actionable? And in an organization with limited engineering bandwidth, what is the most important thing to prioritize?

In this presentation, I aim to provide a practical guide on what I believe will give the greatest "bang for buck" with backup testing, and how to fold it into your operations, modeled after how we test our postgres backups at Academia.edu.

This talk covers:
* What are "physical" backups and what advantages do they offer? (For example: point-in-time recovery out of the box)
* How does one test a "physical" postgres backup?
* What are reasonable goals to set for Recovery Point Objective (RPO) and Recovery Time Objective (RTO) and how do we measure them?
* How to couple the testing of your backups with operations
* What additional monitoring to implement, with a worked example for pgBackRest and Datadog

In addition, I’ll go over the scariest close calls with postgres backups I’ve witnessed and what we can learn from them.
