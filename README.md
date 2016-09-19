# adobe_rum_updaters_for_munki_single-bash
Adobe CC updater scrips for Munki, updates a single CC item only

Items are nopkg-type and they require Adobe RUM command line tool installed on the client computer.
The postinstall_script in pkginfo tries to install update(s) for a specific Adobe CC product defined in the script.
The script has to do some post-install cleaning as running RUM when user is logged in will result to permissions issues as RUM saves the downloaded items to user's home directory.
