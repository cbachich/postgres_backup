# PostgreSQL Backup Script
This script is used to backup all or specific PostgreSQL databases from your local machine. It keeps the latest 7 files and removes older files in the same directory. The number of files it keeps can be changed in the options.

### Usage
````
postgres_backup [options] [DATABASE_NAMES]
````

### Options
````
-n, [--numfiles NUMBER] # Number of files to save (deletes older files)
                        # Default: 7
-a, [--all]             # Save all databases to a single dump file
````

### Example
````
postgres_backup --numfiles 14 -a
````

This generates a single backup of all your databases and keeps up to 14 of those files.
