# linux-management-scripts
Set of scripts to manage Linux servers

SECTIONS:

backup  : Backup scripts
general : General scripts that might be of use
server  : Server management scripts
setup   : Server setup scripts


SCRIPTS:
backup/backup-all    : Main backup script that will execute the backup of everything
backup/backup-server : Will make a backup of the specified server
backup/list-servers  : Will echo a list of currently available servers (currently VERY simply done in a list in a shell script)
backup/setup         : The setup script for a backup server, in case we need to create a new one

general/git-setup : Will configure git for you to have a few nice handy extras

server/deploy : Will execute all required steps on the server to deploy the website to the specified environment (typically production, could be other)
server/lock   : Will lock down the filesystem for security (Used by the deploy script)
server/stage  : Will copy the production version to the specified environment (Typically staging)
server/unlock : Will unlock the filesystem for accessibility (Used by the deploy script) 

setup/setup        : Will setup the specified server
setup/setup-server : Auxiliary script that will be copied to the specified server and executed there to setup the entire server
