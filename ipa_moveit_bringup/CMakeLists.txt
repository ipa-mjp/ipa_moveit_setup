cmake_minimum_required(VERSION 2.8.3)
project(ipa_moveit_bringup)

find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY launch DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

install(PROGRAMS bin/add_robot.sh bin/update_collisions.sh DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})
