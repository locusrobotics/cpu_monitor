^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package cpu_monitor
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.1.0 (2022-02-23)
------------------
* Add dependencies
* Clean up python package
* Update package.xml email address
* Use private namespace for topic names
  Allows topic names to reflect a changing node name.
* Update README
* Add dependency information in README
* Use "python" instead of "python3" in shebang
  This should work on Ubuntu 20.04, where python3 is the default.
* Updates for Python3
* Don't crash if pid cannot be extracted from NODEINFO response
* Fix cases where IP address of process is a superset of the
  ip address of the host (e.g. host == 10.0.0.2 and process running
  on 10.0.0.22)
* Add install info to CMakeLists.txt
* feat(config): make poll period configurable
  Allow the user to specify the poll period. Default value is still 1.0.
* add psutil as a runtime dependency
* Add launch file to launch the cpu_monitor node
* Publish all available virtual memory fields as individual topics
* Better local node checking
* Add README.md
* Become a catkin package: add CMakeLists.txt and package.xml
* Publish memory usage per process as well
  Also publish total CPU and memory usage.
* Initial check in
* Initial commit
* Contributors: Alex Spitzer, Jørgen Borgesen, Kevin Jaget, Matthew Powelson, Paul Bovbel
