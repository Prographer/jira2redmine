<h1>Update to work with latest Jira backup</h1>
I have updated this script to migrate our Jira cloud to Redmine 3.3. In recent backup from Jira, the xml format changed a little bit. 
In Jira cloud, go to System -> Backup and create backup for Jira server.


jira2redmine
============

Script for import from JIRA to redmine

for more information please look at: http://www.redmine.org/issues/1385

## How to

Copy `migrate_jira.rake` to `lib/tasks` in your *Redmine* directory and the execute the following:

```
rake jira_migration:test_all_migrations RAILS_ENV="production"
rake jira_migration:do_all_migrations RAILS_ENV="production"
```
