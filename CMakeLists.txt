cmake_minimum_required(VERSION 2.8.3)
project(cpu_monitor)

find_package(catkin REQUIRED)

catkin_package()

catkin_install_python(
  PROGRAMS scripts/monitor
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})

install(DIRECTORY launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
  PATTERN *~ EXCLUDE
)
