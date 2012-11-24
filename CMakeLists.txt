cmake_minimum_required(VERSION 2.8.3)
project(wstool_catkin)

## Find catkin and any catkin packages on which
## this package depends at build time
find_package(catkin REQUIRED)

## Declare things to be passed to other projects
catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES
#  CATKIN_DEPENDS
#  DEPENDS Boost # other-3rd-party-libraries
)

catkin_add_env_hooks(wstool SHELLS bash zsh DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/env-hooks)
