cmake_minimum_required(VERSION 3.5)
project(ur_controllers)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra)
endif()
set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)

find_package(ament_cmake REQUIRED)
find_package(angles REQUIRED)
find_package(controller_interface REQUIRED)
find_package(geometry_msgs REQUIRED)
find_package(joint_trajectory_controller REQUIRED)
find_package(lifecycle_msgs REQUIRED)
find_package(pluginlib REQUIRED)
find_package(rclcpp_lifecycle REQUIRED)
find_package(rcutils REQUIRED)
find_package(realtime_tools REQUIRED)
find_package(std_msgs REQUIRED)
find_package(std_srvs REQUIRED)
find_package(tf2_geometry_msgs REQUIRED)
find_package(tf2_ros REQUIRED)
find_package(ur_dashboard_msgs REQUIRED)
find_package(ur_msgs REQUIRED)
find_package(generate_parameter_library REQUIRED)
find_package(trajectory_msgs REQUIRED)
find_package(control_msgs REQUIRED)
find_package(action_msgs REQUIRED)


set(THIS_PACKAGE_INCLUDE_DEPENDS
  angles
  controller_interface
  geometry_msgs
  joint_trajectory_controller
  lifecycle_msgs
  pluginlib
  rclcpp_lifecycle
  rcutils
  realtime_tools
  std_msgs
  std_srvs
  tf2_geometry_msgs
  tf2_ros
  ur_dashboard_msgs
  ur_msgs
  generate_parameter_library
  control_msgs
  trajectory_msgs
  action_msgs
)

include_directories(include)

generate_parameter_library(
  tool_contact_controller_parameters
  src/tool_contact_controller_parameters.yaml
)

generate_parameter_library(
  force_mode_controller_parameters
  src/force_mode_controller_parameters.yaml
)

generate_parameter_library(
  gpio_controller_parameters
  src/gpio_controller_parameters.yaml
)

generate_parameter_library(
  speed_scaling_state_broadcaster_parameters
  src/speed_scaling_state_broadcaster_parameters.yaml
)

generate_parameter_library(
  scaled_joint_trajectory_controller_parameters
  src/scaled_joint_trajectory_controller_parameters.yaml
)

generate_parameter_library(
  freedrive_mode_controller_parameters
  src/freedrive_mode_controller_parameters.yaml
)

generate_parameter_library(
  passthrough_trajectory_controller_parameters
  src/passthrough_trajectory_controller_parameters.yaml
)

generate_parameter_library(
  ur_configuration_controller_parameters
  src/ur_configuration_controller_parameters.yaml
)

add_library(${PROJECT_NAME} SHARED
  src/tool_contact_controller.cpp
  src/force_mode_controller.cpp
  src/scaled_joint_trajectory_controller.cpp
  src/speed_scaling_state_broadcaster.cpp
  src/freedrive_mode_controller.cpp
  src/gpio_controller.cpp
  src/passthrough_trajectory_controller.cpp
  src/ur_configuration_controller.cpp)

target_include_directories(${PROJECT_NAME} PRIVATE
  include
)
target_link_libraries(${PROJECT_NAME}
  tool_contact_controller_parameters
  force_mode_controller_parameters
  gpio_controller_parameters
  speed_scaling_state_broadcaster_parameters
  scaled_joint_trajectory_controller_parameters
  freedrive_mode_controller_parameters
  passthrough_trajectory_controller_parameters
  ur_configuration_controller_parameters
  ${geometry_msgs_TARGETS}
  ${lifecycle_msgs_TARGETS}
  ${std_msgs_TARGETS}
  ${std_srvs_TARGETS}
  ${tf2_geometry_msgs_TARGETS}
  ${ur_dashboard_msgs_TARGETS}
  ${control_msgs_TARGETS}
  ${trajectory_msgs_TARGETS}
  ${ur_msgs_TARGETS}
  ${action_msgs_TARGETS}
  angles
  controller_interface
  joint_trajectory_controller
  pluginlib
  rclcpp_lifecycle
  rcutils
  realtime_tools
  tf2_ros
)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  target_compile_options(${PROJECT_NAME} PRIVATE -Wpedantic -Werror)
endif()

# prevent pluginlib from using boost
target_compile_definitions(${PROJECT_NAME} PUBLIC "PLUGINLIB__DISABLE_BOOST_FUNCTIONS")
pluginlib_export_plugin_description_file(controller_interface controller_plugins.xml)

install(TARGETS ${PROJECT_NAME}
  ARCHIVE DESTINATION lib
  LIBRARY DESTINATION lib
  RUNTIME DESTINATION bin
)

install(DIRECTORY include/
  DESTINATION include
)

install(FILES controller_plugins.xml
  DESTINATION share/${PROJECT_NAME}
)

ament_export_dependencies(${THIS_PACKAGE_INCLUDE_DEPENDS})
ament_export_include_directories(include)
ament_export_libraries(${PROJECT_NAME})

ament_export_include_directories(
  include
)

ament_export_libraries(
  ${PROJECT_NAME}
)

if(BUILD_TESTING)
  find_package(ament_cmake_gmock REQUIRED)
  find_package(controller_manager REQUIRED)
  find_package(hardware_interface REQUIRED)
  find_package(ros2_control_test_assets REQUIRED)

  add_definitions(-DTEST_FILES_DIRECTORY="${CMAKE_CURRENT_SOURCE_DIR}/test")
  ament_add_gmock(test_load_force_mode_controller
    test/test_load_force_mode_controller.cpp
  )
  target_link_libraries(test_load_force_mode_controller
    ${PROJECT_NAME}
    controller_manager
    ros2_control_test_assets
  )
  ament_add_gmock(test_load_freedrive_mode_controller
    test/test_load_freedrive_mode_controller.cpp
  )
  target_link_libraries(test_load_freedrive_mode_controller
    ${PROJECT_NAME}
    controller_manager
    ros2_control_test_assets
  )
endif()

ament_package()
