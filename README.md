# unifi-systemd

A systemd unit for starting the unifi controller.

This is a specific config for a specific system, but it includes a list of setup tasks before you can launch the controller.

If you haven't met the dependencies below, this will probably fail epically.

# Quickstart

Copy unifi.service* to /etc/systemd/system

# Dependencies

* unifi user
* unifi apt package
* custom mongodb at /opt/mongodb (omit custom-mongod.conf to disable this behaviour)

# Other weirdness

* If the default JVM_MAX_HEAP_SIZE is set to '1024M', reduce it to '768M' (omit custom-java-mem.conf to disable this behaviour)

 
