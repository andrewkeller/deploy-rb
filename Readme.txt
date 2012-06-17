This is an implementation of deploy, written in REALbasic.

Deploy is a tool used to create a copy of a directory that includes or excludes particular patterns of files and folders.  It is functionally similar to:

	rsync -rt --delete . <destination>

The major difference is that it figures out which files to include or exclude based on configuration files in each folder of the source.

The usage of deploy is as follows:

	deploy <target> <destination>

The target and destination parameters must be supplied for every invocation, unless a default value has been set in one of the configuration files.  In a properly set up project, you can usually run `deploy`, and it will deploy the default target to the default destination.
