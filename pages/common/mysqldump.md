# mysqldump

> Backups MySQL databases.
> More information: <https://dev.mysql.com/doc/refman/en/mysqldump.html>.

- Create a backup (user will be prompted for a password):

`mysqldump --user {{user}} --password {{database_name}} -r {{path/to/file.sql}}`

- Restore a backup (user will be prompted for a password):

`mysqldump --user {{user}} --password {{database_name}} < {{path/to/file.sql}}`

- Backup all databases redirecting the output to a file (user will be prompted for a password):

`mysqldump --user {{user}} --password --all-databases > {{path/to/file.sql}}`

- Restore all databases from a backup (user will be prompted for a password):

`mysqldump --user {{user}} --password < {{path/to/file.sql}}`
