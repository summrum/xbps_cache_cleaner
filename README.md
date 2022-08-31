# xbps Cache Cleaner

Shell script used for cleaning the xbps cache of uninstalled and/or outdated packages on Void linux. 

The script will search through ```/var/cache/xbps/``` for any packages not currently installed on the system, write a file with any found entries to ```/tmp/cache_cleaner.txt```, open that file in ```less```, then offer to delete all found packages (and corresponding signatures) after the file is closed.

If the user chooses not to let the script delete any found packages and signatures, the temporary file ```/tmp/cache_cleaner.txt``` will not be deleted after the script exits (otherwise it will be).
