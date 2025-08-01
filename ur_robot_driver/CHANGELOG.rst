4.1.0 (2025-07-29)
------------------
* Migrate hardware_interface's on_init method (`#1464 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1464>`_)
* Add scaling parameters to upstream JTC (`#1465 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1465>`_)
* Add migration of ros2_control node to migration notes (`#1458 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1458>`_)
* Fix flaky controller switch test (`#1447 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1447>`_)
* fix_flaky_force_mode_test (`#1429 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1429>`_)
* Reduce flakiness of trajectory controller tests (`#1443 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1443>`_)
* Added 'is in remote control' call as a dashboard service (`#1433 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1433>`_)
* ur_robot_driver: Fix compilation on Windows (`#1421 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1421>`_)
* Refactor prepare_switch method (`#1417 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1417>`_)
* Update simulation page to also explicitly mention PolyScope X (`#1415 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1415>`_)
* Contributors: Felix Exner, Mads Holm Peters, Silvio Traversaro

4.0.3 (2025-06-16)
------------------

4.0.2 (2025-06-13)
------------------
* Remove unnecessary arguments. (`#1389 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1389>`_)
* Contributors: Dr. Denis

4.0.1 (2025-05-28)
------------------
* [force mode controller] Fix the task frame orientation (`#1379 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1379>`_)
* Replace ament_target_dependencies calls (`#1373 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1373>`_)
* Update feature list (`#1372 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1372>`_)
* Contributors: Felix Exner

4.0.0 (2025-05-20)
------------------
* Add support for UR15 (`#1358 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1358>`_)
* [CI] Check links using lychee instead of a custom script (`#1355 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1355>`_)
* Make check_starting_point of test_move launch files configurable (`#1354 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1354>`_)
* Add troubleshooting section about handling ABI breaks (`#1350 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1350>`_)
* Only append to start_modes in prepare_switch (`#1344 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1344>`_)
* tool_contact_test: Check result status directly (`#1345 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1345>`_)
* Contributors: Felix Exner

3.2.1 (2025-04-11)
------------------
* Disable enforcing command limits (`#1342 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1342>`_)
* Contributors: Felix Exner

3.2.0 (2025-04-10)
------------------
* Added controller to enable and disable tool contact (`#940 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/940>`_)
* Start executing passthrough trajectories earlier than all points are transferred. (`#1313 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1313>`_)
* Support PolyScopeX robots (`#1318 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1318>`_)
* Add support for UR7e and UR12e (`#1320 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1320>`_)
* Use UrDriverConfig struct to initialize UrDriver (`#1328 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1328>`_)
* Fix passthrough controller to not read non-existing state_interfaces (`#1314 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1314>`_)
* Fix links to forward command controllers (`#1303 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1303>`_)
* Contributors: Felix Exner, URJala

3.1.1 (2025-03-17)
------------------
* Update transformForceTorque to handle whether it is a cb3 or an e-Series robot (`#1287 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1287>`_)
* Update message documentation URLs (`#1292 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1292>`_)
* Contributors: Felix Exner

3.1.0 (2025-03-05)
------------------
* Port robot_state_helper to ROS2 (`#933 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/933>`_)
* Fix crashes on shutting down (`#1270 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1270>`_)
* Fix formatting (`#1262 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1262>`_)
* Move some documentation to client_library (`#1245 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1245>`_)
* Contributors: Felix Durchdewald, Felix Exner

3.0.2 (2025-01-21)
------------------
* Check quaternions for equal dot_product instead of comparing their components individually (`#1238 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1238>`_)
* fix sphinx doc link in ur_robot_driver (`#1240 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1240>`_)
* Disable pose broadcaster on mock hardware (`#1229 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1229>`_)
* Add information about which driver features dont work with mock hardware (`#1227 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1227>`_)
* Add instructions for enabling necessary services and remote control (`#1224 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1224>`_)
* Contributors: Felix Exner, Rune Søe-Knudsen, URJala

3.0.1 (2024-12-30)
------------------
* Remove unused include (`#1220 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1220>`_)
* improve docs around usage of extracted calibration info (`#1214 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1214>`_)
* Contributors: Bence Magyar, Carter Sifferman

3.0.0 (2024-12-18)
------------------
* Freedrive Controller (`#1114 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1114>`_)
* Fix running force_mode controller alongside passthrough trajectory controller (`#1210 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1210>`_)
* Update package maintainers (`#1203 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1203>`_)
* Add force mode controller (`#1049 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1049>`_)
* Add trajectory passthrough controller (`#944 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/944>`_)
* Use pose_broadcaster to publish the TCP pose (`#1108 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1108>`_)
* Contributors: Felix Exner, URJala, Vincenzo Di Pentima

2.4.13 (2024-10-28)
-------------------
* Fix component lifecycle (`#1098 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1098>`_)
* Add missing state interfaces for get_robot_software_version (`#1153 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1153>`_)
* Contributors: Felix Exner (fexner)

2.4.12 (2024-10-14)
-------------------
* Revert "Add passthrough interfaces for joints (`#1121 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1121>`_)" (`#1151 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1151>`_)
* Contributors: Felix Exner (fexner)

2.4.11 (2024-10-10)
-------------------
* Add note about TEM (`#1136 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1136>`_)
* Allow setting the analog output domain when setting an analog IO (`#1123 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1123>`_)
* Service to get software version of robot (`#964 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/964>`_)
* Add passthrough interfaces for joints (`#1121 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1121>`_)
* Fix for Controller Switching Issue and Refactor Controller Spawning (`#1093 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1093>`_)
* Improve usage documentation (`#1110 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1110>`_)
* Assure the description is loaded as string (`#1106 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1106>`_)
* Contributors: Chen Chen, Felix Exner (fexner), URJala

2.4.10 (2024-09-11)
-------------------
* Fix for forward_velocity_controller test (`#1076 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1076>`_)
* Update maintainers team (`#1088 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1088>`_)
* Contributors: Vincenzo Di Pentima

2.4.9 (2024-08-09)
------------------
* Added dynamics tag when using mock_components/GenericSystem (`#1075 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1075>`_)
* Updated the UR family photo on the readme (`#1064 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1064>`_)
* Fix passing launch_dashboard_client launch argument (`#1057 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1057>`_)
* [doc] Add more documentation regarding usage (`#1055 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1055>`_)
* Add doc to custom URScript commands that it needs to be in headless mode (`#1051 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1051>`_)
* Update reference to ros2_controllers test node (`#1054 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1054>`_)
* [doc] Update required polyscope version (`#1052 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1052>`_)
* Add migration notes for jazzy (`#1045 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1045>`_)
* Contributors: Felix Exner (fexner), Rune Søe-Knudsen

2.4.8 (2024-07-01)
------------------
* Add sleep between controller stopper's controller queries (`#1038 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1038>`_)
* Contributors: Felix Exner (fexner)

2.4.7 (2024-06-19)
------------------
* Fix launching without a tf_prefix specified (`#1029 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1029>`_)
* Contributors: Felix Exner (fexner)

2.4.6 (2024-06-17)
------------------
* Remove tf_prefix from ur_control.launch.py (`#1020 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1020>`_)
* Make moveit_config compatible to moveit_configs_builder (`#998 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/998>`_)
* Remove extra spaces from start_ursim statement in tests (`#1010 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/pull/1010>`_)
* Replace keepalive count (`#1002 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/1002>`_)
* Restructure documentation for full stack documentation (`#984 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/984>`_)
* Contributors: Felix Exner, Ruddick Lawrence, Vincenzo Di Pentima

2.4.5 (2024-05-16)
------------------
* Remove dependency to docker.io (`#985 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/985>`_)
* Move starting the robot_state_publisher to an own launch file (`#977 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/977>`_)
  Co-authored-by: Vincenzo Di Pentima <DiPentima@fzi.de>
* Update installation instructions for source build (`#967 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/967>`_)
* Fix multi-line strings in DeclareLaunchArgument (`#948 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/948>`_)
* Contributors: Christoph Fröhlich, Felix Exner (fexner), Matthijs van der Burgh

2.4.4 (2024-04-04)
------------------
* Use ros2 control node from controller_manager and description topic (`#939 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/pull/939>`_)
* Move communication setup to on_configure instead of on_activate (`#732 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/732>`_)
* [URDF] Fix initial value of speed scaling factor syntax (`#920 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/920>`_)
* Reduce number of controller_spawners to 3 (`#919 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/pull/919>`_)
* Contributors: Felix Exner

2.4.3 (2024-02-02)
------------------
* Add UR30 support (`#899 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/899>`_)
* Add control description and ros2_control tag to driver. (`#877 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/877>`_)
* Contributors: Felix Exner (fexner)

2.4.2 (2023-11-23)
------------------
* [README] Move installation instructions to subpage (`#870 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/870>`_)
* Add backward_ros to driver (`#872 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/872>`_)
* Simplify tests (`#849 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/849>`_)
* Port configuration  (`#835 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/835>`_)
  Added possibility to change the reverse_port, script_sender_port and trajectory_port
* [README] Update link to MoveIt! documentation
* Do not start urscipt_interface when using mock hardware
* Contributors: Felix Durchdewald, Felix Exner, RobertWilbrandt

2.4.1 (2023-09-21)
------------------
* Added a test that sjtc correctly aborts on violation of constraints (`#810 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/pull/810>`_)
* Added support for UR20 (`#797 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/797>`_)
* Contributors: Felix Exner

2.4.0 (2023-08-28)
------------------
* Start ursim from lib (`#733 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/733>`_)
  * Forward start_ursim.sh to the one from the client library
  * Update docs and tests to start ursim from the ur_client_library script
* Update velocity-control on feature list (`#573 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/573>`_)
  ros2_controllers jtc does support velocity control by now, so we should not state it doesn't.
* Introduced tf_prefix into log handler (`#713 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/713>`_)
  * Introduced tf_prefix into log handler
  * added default argument to prefix
  ---------
  Co-authored-by: Lennart Nachtigall <firesurfer@firesurfer.de>
  Co-authored-by: Felix Exner <exner@fzi.de>
  Co-authored-by: Lennart Nachtigall <lennart.nachtigall@sci-mo.de>
* Run robot driver test also with tf_prefix (`#729 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/729>`_)
  * Run robot driver test also with tf_prefix
  * Use tf_prefix substitution in controllers config file
  * Set default value of tf_prefix in launchfile to empty instead of '""'
  ---------
  Co-authored-by: Robert Wilbrandt <wilbrandt@fzi.de>
* Use mock_hardware and mock_sensor_commands instead of fake (`#739 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/739>`_)
  * Use mock_hardware and mock_sensor_commands instead of fake
  This has been deprecated a while back and was never adapted.
  * Update documentation to mock_hardware
* Urscript interface (`#721 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/721>`_)
  * Add a urscript interface node
  * Add urscript_interface to standard launchfile
  * Added documentation for urscript_interface
  * Add a notice about incorrect script code
  * Add test for urscript interface
  * Move tests to one single tests
  This should avoid that different tests run in parallel
  * Wait for IO controller before checking IOs
  * Write an initial textmessage when connecting the urscript_interface
  * Wait for controller_manager services longer
  * Make sure we have a clean robot state without any program running once we enter our test
  similar to how we did it on the robot_driver test
  * Remove unneeded Destructor definition
* Use SCHED_FIFO for controller_manager's main thread (`#719 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/719>`_)
  Previous investigations showed that using FIFO scheduling helps keeping
  cycle times also non non-RT kernels. This combined with non-blocking read
  can result in a very stable system.
  This is, in fact, very close to what the actual controller_manager_node
  does except that we always use FIFO scheduling independent of the actual
  kernel in use.
* Contributors: Felix Exner (fexner), Lennart Nachtigall

2.3.2 (2023-06-02)
------------------
* Adds full nonblocking readout support (Multiarm part 4)  - v2 (`#673 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/673>`_)
* Removed workaround also in export_command_interfaces (`#692 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/692>`_)
* Calling on_deactivate in dtr (`#679 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/679>`_)
* Fixed formatting (`#685 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/685>`_)
* Remove tf_prefix workaround in hw interface
* Ported controllers to generate_parameters library and added prefix for controllers (Multiarm part 2) (`#594 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/594>`_)
* Remove ur_bringup package (`#666 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/666>`_)
* Introduce hand back control service (`#528 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/528>`_)
* Apply suggestions from code review
* Update definition of test goals to new version.
* Wait longer for controllers to load and activate
* Fix flaky tests (`#641 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/641>`_)
  * Move robot startup into test's setUp function
  * Robustify robot startup
* This commits adds additional configuration parameters needed for multiarm support.
* Add timeout to execution test
* Improve logging for robot execution tests
* Contributors: Denis Štogl, Dr. Denis, Felix Exner, Felix Exner (fexner), Lennart Nachtigall, Robert Wilbrandt, livanov93

2.3.1 (2023-03-16)
------------------
* Adjust controller switching to message change
* Controller spawner timeout (`#608 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/608>`_)
  * Simplify controller spawner definitions
  * Ignore flake8 W503 as it clashes with black and goes against PEP8 style
  * Add argument to set controller spawner timeout
  * Use longer controller manager timeout in CI
  The default timeout of 10s is the same as our RTDE retry timeout, which
  means if RTDE does not immediately connect (which happens regularly in
  CI runners) controller spawning would fail.
* Increase timeout for first test service call to driver (`#605 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/605>`_)
* Contributors: Robert Wilbrandt, RobertWilbrandt

2.3.0 (2023-03-02)
------------------
* Fix cmake dependency on controller_manager
* Correct calibration correction launch file in doc
* Added services to set tool voltage and zero force torque sensor (`#466 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/466>`_)
  Added launch arguments for reverse ip and script command interface port.
* Fix comment in test file
* Default path to ur_client_library urscript (`#316 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/316>`_)
  * Change default path for urscript for headless mode.
  * Replace urscript path also in newer ur_robot_driver launchfile
  * Remove ros_control.urscript
  Co-authored-by: Felix Exner <exner@fzi.de>
* Clean up & improve execution tests (`#512 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/512>`_)
  * Clean up execution test files
  * Start ursim as part of the execution tests
  * Dont use custom dockerursim for humble and rolling execution tests
  * Clean up test implementations
  * pep257 fixes
  * Perform rolling and humble execution tests as part of normal pipelines
  * Increase admissible timeouts as the CI needs to pull ursim first
  * Add more debug messages during tests
  * Wait until robot is in POWER_OFF mode before trying to power it on
  * Fix error introduced in last commit
  * Add additional cmake option to enable integration tests
  * Increase timeout for robot tests
  * Add CMake comment describing the execution test integration
  * Run source tests on pull request
  This is only here for testing the test setup! Remove before merging
  * call resend_robot_program twice
  This seems to be necessary, as otherwise the robot hangs after bootup.
  The first program execution (that gets automatically started at driver
  startup because of the headless_mode) gets paused, since it is sent while
  the robotis not yet switched on. To mitigate this, we send the robot program
  again after switching on the robot, but this seems to stop the robot program.
  Sending it again seems to set it correctly to a started state.
  * Increase timeouts for dashboard_client tests
  Otherwise they can fail, since in parallel we pull and start the docker
  container.
  Co-authored-by: Felix Exner <exner@fzi.de>
* Update and thin down README (`#494 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/494>`_)
  Avoid duplication between README and package doc.
  * Updated documentation about fake_hardware and MoveIt!
  * Remove trailing WS
  * [documentation] do not suggest -r for rosdep install
  * Added note about tool0_controller to docs.
  * Add additional part about calibration to toplevel README.
  * Added note about sourcing ROS in build instructions
* ur_robot_driver: Controller_stopper fix deprecation warning
  Use ``activate_controllers`` instead of ``start_controllers``.
* Fix tool voltage setup (`#526 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/526>`_)
  * Move BEGIN_REPLACE inside of header
  * Change default value of tool_voltage
  Keeping this at 0 requires users to explicitly set it to non-zero. This way
  we won't accitentally destroy hardware that cannot handle 24V.
* Added dependency to socat (`#527 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/527>`_)
  This is needed for the tool forwarding.
* Add a note in the tool_comm doc about a URCap conflict (`#524 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/524>`_)
  * Add a note in the tool_comm doc about a URCap conflict
  * Update ur_robot_driver/doc/setup_tool_communication.rst
  Co-authored-by: Mads Holm Peters <79145214+urmahp@users.noreply.github.com>
  * Fix formatting and one spelling mistake
  Co-authored-by: Mads Holm Peters <79145214+urmahp@users.noreply.github.com>
* Contributors: Felix Exner, Felix Exner (fexner), Mads Holm Peters, Robert Wilbrandt, RobertWilbrandt, livanov93

2.2.4 (2022-10-07)
------------------
* Remove the custom ursim docker files (`#478 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/478>`_)
  This has been migrated inside the docs and is not needed anymore.
* Remove duplicated update_rate parameter (`#479 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/479>`_)
* Contributors: Felix Exner

2.2.3 (2022-07-27)
------------------
* Adapt ros control api (`#448 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/448>`_)
  * scaled jtc: Use get_interface_name instead of get_name
  * Migrate from stopped controllers to inactive controllers
  stopped controllers has been deprecated upstream
* Contributors: Felix Exner

2.2.2 (2022-07-19)
------------------
* Made sure all past maintainers are listed as authors (`#429 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/429>`_)
* Silence a compilation warning (`#425 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/425>`_)
  Since setting the receive timeout takes the time_buffer as an argument
  this raises a "may be used uninitialized" warning. Setting this to 0
  explicitly should prevent that.
* Doc: Fix IP address in usage->ursim section (`#422 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/422>`_)
* Contributors: Felix Exner

2.2.1 (2022-06-27)
------------------
* Fixed controller name for force_torque_sensor_broadcaster (`#411 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/411>`_)
* Contributors: Felix Exner

2.2.0 (2022-06-20)
------------------
* Updated package maintainers
* Rework bringup (`#403 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/403>`_)
* Prepare for humble (`#394 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/394>`_)
* Update dependencies on all packages (`#391 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/391>`_)
* Update HW-interface API for humble. (`#377 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/377>`_)
* Use types in hardware interface from ros2_control in local namespace (`#339 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/339>`_)
* Update header extension to remove compile warning. (`#285 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/285>`_)
* Add resource files from ROS World. (`#226 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/226>`_)
* Add sphinx documentation (`#340 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/340>`_)
* Update license to BSD-3-Clause (`#277 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/277>`_)
* Update ROS_INTERFACE.md to current driver (`#335 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/335>`_)
* Fix hardware interface names in error output (`#329 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/329>`_)
* Added controller stopper node (`#309 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/309>`_)
* Correct link to calibration extraction (`#310 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/310>`_)
* Start the tool communication script if the flag is set (`#267 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/267>`_)
* Change driver constructor and change calibration check (`#282 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/282>`_)
* Use GPIO tag from URDF in driver. (`#224 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/224>`_)
* Separate control node (`#281 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/281>`_)
* Add missing dependency on angles and update formatting for linters. (`#283 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/283>`_)
* Do not print an error output if writing is not possible (`#266 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/266>`_)
* Update features.md (`#250 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/250>`_)
* Tool communication (`#218 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/218>`_)
* Payload service (`#238 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/238>`_)
* Import transformation of force-torque into tcp frame from ROS1 driver (https://github.com/UniversalRobots/Universal_Robots_ROS_Driver/blob/master/ur_robot_driver/src/hardware_interface.cpp). (`#237 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/237>`_)
* Make reading and writing work when hardware is disconnected (`#233 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/233>`_)
* Add missing command and state interfaces to get everything working with the fake hardware and add some comment into xacro file to be clearer. (`#221 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/221>`_)
* Decrease the rate of async tasks. (`#223 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/223>`_)
* Change robot type. (`#220 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/220>`_)
* Driver to headless. (`#217 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/217>`_)
* Test execution tests (`#216 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/216>`_)
* Integration tests improvement (`#206 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/206>`_)
* Set start modes to empty. Avoid position ctrl loop on start. (`#211 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/211>`_)
* Add resend program service and enable headless mode (`#198 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/198>`_)
* Implement "choices" for robot_type param (`#204 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/204>`_)
* Calibration extraction package (`#186 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/186>`_)
* Add breaking api changes from ros2_control to hardware_interface (`#189 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/189>`_)
* Fix prepare and perform switch operation (`#191 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/191>`_)
* Update CI configuration to support galactic and rolling (`#142 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/142>`_)
* Dockerize ursim with driver in docker compose (`#144 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/144>`_)
* Enabling velocity mode (`#146 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/146>`_)
* Moved registering publisher and service to on_active (`#151 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/151>`_)
* Converted io_test and switch_on_test to ROS2 (`#124 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/124>`_)
* Added loghandler to handle log messages from the Client Library with … (`#126 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/126>`_)
* Removed dashboard client from hardware interface
* [WIP] Updated feature list (`#102 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/102>`_)
* Moved Async check out of script running check (`#112 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/112>`_)
* Fix gpio controller (`#103 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/103>`_)
* Fixed speed slider service call (`#100 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/100>`_)
* Adding missing backslash and only setting workdir once (`#108 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/108>`_)
* Added dockerfile for the driver (`#105 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/105>`_)
* Using official Universal Robot Client Library (`#101 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/101>`_)
* Reintegrating missing ur_client_library dependency since the break the building process (`#97 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/97>`_)
* Fix readme hardware setup (`#91 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/91>`_)
* Fix move to home bug (`#92 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/92>`_)
* Using modern python
* Some intermediate commit
* Remove obsolete and unused files and packages. (`#80 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/80>`_)
* Review CI by correcting the configurations (`#71 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/71>`_)
* Add support for gpios, update MoveIt and ros2_control launching (`#66 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/66>`_)
* Quickfix against move home bug
* Added missing initialization
* Use GitHub Actions, use pre-commit formatting (`#56 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/56>`_)
* Put dashboard services into corresponding namespace
* Start dashboard client from within the hardware interface
* Added try catch blocks for service calls
* Removed repeated declaration of timeout parameter which lead to connection crash
* Removed static service name in which all auto generated services where mapped
* Removed unused variable
* Fixed clang-format issue
* Removed all robot status stuff
* Exchanged hardcoded value for RobotState msgs enum
* Removed currently unused controller state variables
* Added placeholder for industrial_robot_status_interface
* Fixed clang issues
* Added checks for internal robot state machine
* Only load speed scaling interface
* Changed state interface to combined speed scaling factor
* Added missing formatting in hardware interface
* Initial version of the speed_scaling_state_controller
* Fix clang tidy in multiple pkgs.
* Clang tidy fix.
* Update force torque state controller.
* Prepare for testing.
* Fix decision breaker for position control. Make decision effect instantaneous.
* Use only position interface.
* Update hardware interface for ROS2 (`#8 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/8>`_)
* Update the dashboard client for ROS2 (`#5 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/5>`_)
* Hardware interface framework (`#3 <https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/issues/3>`_)
* Add XML schema to all ``package.xml`` files
* Silence ``ament_lint_cmake`` errors
* Update packaging for ROS2
* Update package.xml files so ``ros2 pkg list`` shows all pkgs
* Clean out ur_robot_driver for initial ROS2 compilation
* Compile ur_dashboard_msgs for ROS2
* Delete all launch/config files with no UR5 relation
* Initial work toward compiling ur_robot_driver
* Update CMakeLists and package.xml for:
  - ur5_moveit_config
  - ur_bringup
  - ur_description
* Change pkg versions to 0.0.0
* Contributors: AndyZe, Denis Stogl, Denis Štogl, Felix Exner, John Morris, Lovro, Mads Holm Peters, Marvin Große Besselmann, Rune Søe-Knudsen, livanov93, Robert Wilbrandt

0.0.3 (2019-08-09)
------------------
* Added a service to end ROS control from ROS side
* Publish IO state on ROS topics
* Added write channel through RTDE with speed slider and IO services
* Added subscriber to send arbitrary URScript commands to the robot

0.0.2 (2019-07-03)
------------------
* Fixed dependencies and installation
* Updated README
* Fixed passing parameters through launch files
* Added support for correctly switching controllers during runtime and using the standard
  joint_trajectory_controller
* Updated externalcontrol URCap to version 1.0.2
  + Fixed Script timeout when running the URCap inside of a looping tree
  + Fixed a couple of typos
* Increased minimal required UR software version to 3.7/5.1

0.0.1 (2019-06-28)
------------------
Initial release
