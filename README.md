# `autorsync` for Linux

Automatically keep a local directory in sync with a remote directory.
It automatically executes rsync for each inotify-event.
This is supposed to run on a slave-machine, to ensure that the local slave-directory is always ready for taking over the remote master-directory on the master-machine.


Note that this is a dumb script, it only does the synchronization.
Taking care of automatic fail-over, and electing a new master in a pool of machines should be implemented by a separate program.

# Dependencies

 - `bash`
 - `inotify-tools`
 - `rsync`
 - `ssh`
