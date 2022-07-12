# interview_test
In this repositery you can find the solutions for tasks discribed in tasks.pdf each file contains a script realted to a specific a task

```requirements.txt``` contains the required Python packages for the tasks

### Notes: 
- Task 4 : In task 4 there is an issue : to convert from USD to EUR according a specific day i need the conversion rate for each day which i collected from eurofxref-hist-90d.xml but not all dates that existing transaction DB are covered so for some dates(example:2019-11-02) we don't have the conversion rate so when i updated the table i supposed that the conversion rate is 1 for those dates . this solution is just for this test in a real project i would use an updated version from the eurofxref-hist-90d.xml and make sure that it contains all the dates in the time frame of the recorded transactions

- Task 5 : There is two approaches :
1. starting from scratch and want to use Postgres instead of sqlite but this would be time consuming and not practical 
2. We have an already populated sqliteDB so we need only need to migrate it to Postgres.

Adopting the second approach i used [this tutorial](https://www.enterprisedb.com/postgresql-tutorial-resources-training?uuid=db55e32d-e9f0-4d7c-9aef-b17d01210704&campaignId=7012J000001NhszQAC)

