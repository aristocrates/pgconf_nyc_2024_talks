# Nick Meyer's PGConf NYC 2024 talks

## Academia.edu is hiring

See https://www.academia.edu/hiring?pgconfnyc=nickmeyer for more details.

Or if you prefer no URL param: https://www.academia.edu/hiring

## 9.2 to 15 and beyond: a case study of a tricky upgrade path

Wednesday, 2024-10-02 11:40 UTC -4:00

https://postgresql.us/events/pgconfnyc2024/schedule/session/1819-92-to-15-and-beyond-a-case-study-of-a-tricky-upgrade-path/

Some signs that you may want to think about upgrading postgres:
* You have to click on the “Unsupported versions” row to double check everything you read in the docs
* You hear about a feature that has been around since postgres 11 (or 9.3) and wish that you were able to use it
* Whenever you mention the version you are running, people mention how out of date it is

While there is a lot of advice emphasizing the benefits of upgrading, sometimes it can feel like there are fewer details on how to deal with trickier situations you may be in. I hope to partially fill this niche with our story of how we at Academia.edu went from 9.2 to 15.

In this talk we will cover:
* Running `pg_upgrade` when you have streaming replicas and want to minimize downtime
* Using pglogical with DDL replication and the challenges that come with it 
* Various complications that occurred along this journey
* Greatest technical frustrations I have experienced while upgrading
* My personal list of favorite new features from 9.3 to 15

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
