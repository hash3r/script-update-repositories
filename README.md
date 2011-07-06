Script: Update Repositories
=============

The intended purpose of this script is to allow developers to come into the office
and run one script that goes through all of their projects and grabs the latest data.

Example usage:

$ pwd
/Users/username/Projects/

$ chmod +x update-repositories.rb

echo 'These will all do the same thing!'

$ ./update-repositories.rb .
$ ./update-repositories.rb ~/username/Projects/
$ ./update-repositories.rb /Users/username/Projects/

Example output:

`
$ ./update-repositories.rb .
# Checking given path.,,
# [ SUCCESS ] .

# Checking: ror:morange
Pulling: origin -> gitosis@git.myserver.com:morange.git 

# Already up-to-date.

# Checking: ror:orange
Pulling: origin -> gitosis@git.myserver.com:orange.git 

# Already up-to-date.

# Checking: sandbox
[ FAIL ] Unable to locate any remote branches.

# Checking: slice17.myserver.com:assets:blogs.dir
Pulling: origin -> gitosis@git.myserver.com:blogs.dir.git 

# Already up-to-date.

# Checking: wordpress
Pulling: origin -> git@github.com:myserver/wordpress.git 

# Already up-to-date.

# Checking: wordpress-plugin:myserver-plugin
Pulling: origin -> gitosis@git.myserver.com:myserver-plugin.git 

# Already up-to-date.

# Checking: wordpress-plugin:myserver-widgets
Pulling: origin -> gitosis@git.myserver.com:myserver-widgets.git 

# Already up-to-date.

# Checking: wordpress-plugin:inventory-api
Pulling: origin -> git@github.com:myserver/wordpress-plugin-inventory-api.git 

# Already up-to-date.

# Checking: wordpress-plugin:staff-listing
Pulling: origin -> git@github.com:myserver/wordpress-plugin-staff-listing.git 

# Already up-to-date.

# Checking: wordpress-plugin:wiget-enhancements
Pulling: origin -> gitosis@git.myserver.com:widget-enhancements 

# Already up-to-date.

# Checking: wordpress-theme:cardealerpress
Pulling: origin -> gitosis@git.myserver.com:myserver-theme.git 

# Already up-to-date.

# Checking: wordpress-theme:myserver-themes
Pulling: origin -> gitosis@git.myserver.com:wordpress-themes.git 

# Already up-to-date.

# Do work son!
`
