# PostgreSQL_update
PostgreSQL from version 14 to 15

necessary steps for upgrading PostgreSQL from version 14 to 15
error checking to ensure every step is successful before proceeding to the next one.
It's better to use sudo -u postgres to run commands as the postgres user rather than switching to the user with sudo su - postgres.
You should backup the databases before starting the upgrade.
You should reload the PostgreSQL service after changing the port.
Removing old packages should be done using purge instead of remove to also delete configuration and/or data files.
The delete_old_cluster.sh script is in the PostgreSQL you can point the last command to this or just leave it commented out and it will switch user and run . we should ensure it's available and executable.
Please replace "/path/to/your/delete_old_cluster.sh" with the actual path of the script.
