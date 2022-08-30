# xbps_cache_cleaner

Shell script used for cleaning the xbps cache of uninstalled and/or outdated packages on Void linux. The script will search through ```/var/cache/xbps/``` for any packages not currently installed on the system, write a file with any found entries to ```/tmp/```, open that file in ```less```, then offer to delete any found packages (and corresponding signatures) after the file is closed.
