# Project Tour

* notes:
*  > Discuss about your project file structure
*  > what each folder is responsible
*  > then go through each file in folders and explain there purpose
*  > if possible create a doc system ( there are autogen docs available for most of the languages )
*  > decide coding style , linting style and formatting style and other themes like variable naming etc.
*  > provide an example for existing function and tests system if possible
   > The folders one should be most concerned with are :-
     turtlebot3_gazebo --> launch, worlds
*  Folder Structure of src is as follows:-
.
├── LICENSE
├── README.md
├── turtlebot3_fake
│   ├── CHANGELOG.rst
│   ├── CMakeLists.txt
│   ├── include
│   │   └── turtlebot3_fake
│   │       └── turtlebot3_fake.h
│   ├── launch
│   │   └── turtlebot3_fake.launch
│   ├── package.xml
│   ├── rviz
│   │   └── turtlebot3_fake.rviz
│   └── src
│       └── turtlebot3_fake.cpp
├── turtlebot3_gazebo
│   ├── CHANGELOG.rst
│   ├── CMakeLists.txt
│   ├── include
│   │   └── turtlebot3_gazebo
│   │       └── turtlebot3_drive.h
│   ├── launch
│   │   ├── multi_map_merge.launch
│   │   ├── multi_turtlebot3.launch
│   │   ├── multi_turtlebot3_slam.launch
│   │   ├── turtlebot3_autorace_2020.launch
│   │   ├── turtlebot3_autorace.launch
│   │   ├── turtlebot3_autorace_mission.launch
│   │   ├── turtlebot3_empty_world.launch
│   │   ├── turtlebot3_gazebo_rviz.launch
│   │   ├── turtlebot3_house.launch
│   │   ├── turtlebot3_simulation.launch
│   │   ├── turtlebot3_stage_1.launch
│   │   ├── turtlebot3_stage_2.launch
│   │   ├── turtlebot3_stage_3.launch
│   │   ├── turtlebot3_stage_4.launch
│   │   └── turtlebot3_world.launch
│   ├── models
│   │   ├── turtlebot3_autorace
│   │   │   ├── course
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── course.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── course.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_bar_down
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_bar.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── traffic_bar.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_bar_up
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_bar.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── traffic_bar.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_light_green
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_light_red
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_light_yellow
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_parking
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_parking.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── traffic_parking.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_stop
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_stop.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── traffic_stop.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   └── traffic_tunnel
│   │   │       ├── materials
│   │   │       │   ├── scripts
│   │   │       │   │   └── tunnel.material
│   │   │       │   └── textures
│   │   │       │       └── tunnel.png
│   │   │       ├── model.config
│   │   │       └── model.sdf
│   │   ├── turtlebot3_autorace_2020
│   │   │   ├── checker
│   │   │   │   ├── materials
│   │   │   │   │   ├── checker.png
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── checker.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── checker.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── course
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── course.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── course.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_bar_down
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_bar_down.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── traffic_bar_down.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_bar_up
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_bar_up.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── traffic_bar_up.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_construction
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_construction.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_construction.png
│   │   │   │   │       └── traffic_construction_white_background.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_intersection
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_intersection.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_intersection.png
│   │   │   │   │       └── traffic_intersection_white_background.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_left
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_is_left.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_left.png
│   │   │   │   │       └── traffic_left_white_background.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_light_green
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_light_green.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── traffic_light_green.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_light_red
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_light_red.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_light.png
│   │   │   │   │       └── traffic_light_red.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_light_yellow
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_light_yellow.material
│   │   │   │   │   └── textures
│   │   │   │   │       └── traffic_light_yellow.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_noentry
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_noentry.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_noentry.png
│   │   │   │   │       └── traffic_noentry_white_background.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_parking
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_parking.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_parking.png
│   │   │   │   │       └── traffic_parking_white_background.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_pl_left
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_pl_left.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_pl_left.png
│   │   │   │   │       └── traffic_pl_left_white_background.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_right
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_right.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_right.png
│   │   │   │   │       └── traffic_right_white_background.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── traffic_stop
│   │   │   │   ├── materials
│   │   │   │   │   ├── scripts
│   │   │   │   │   │   └── traffic_stop.material
│   │   │   │   │   └── textures
│   │   │   │   │       ├── traffic_stop.png
│   │   │   │   │       └── traffic_stop_white_background.png
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   └── traffic_tunnel
│   │   │       ├── materials
│   │   │       │   ├── scripts
│   │   │       │   │   └── tunnel.material
│   │   │       │   └── textures
│   │   │       │       ├── tunnel.png
│   │   │       │       └── tunnel_white_background.png
│   │   │       ├── model.config
│   │   │       └── model.sdf
│   │   ├── turtlebot3_burger
│   │   │   ├── model-1_4.sdf
│   │   │   ├── model.config
│   │   │   └── model.sdf
│   │   ├── turtlebot3_common_meshes
│   │   │   ├── burger_base.dae
│   │   │   ├── lds.dae
│   │   │   ├── r200.dae
│   │   │   ├── tire.dae
│   │   │   ├── waffle_base.dae
│   │   │   └── waffle_pi_base.dae
│   │   ├── turtlebot3_house
│   │   │   ├── model.config
│   │   │   └── model.sdf
│   │   ├── turtlebot3_plaza
│   │   │   ├── goal_box
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── model.config
│   │   │   └── model.sdf
│   │   ├── turtlebot3_square
│   │   │   ├── goal_box
│   │   │   │   ├── model.config
│   │   │   │   └── model.sdf
│   │   │   ├── model.config
│   │   │   └── model.sdf
│   │   ├── turtlebot3_waffle
│   │   │   ├── model-1_4.sdf
│   │   │   ├── model.config
│   │   │   └── model.sdf
│   │   ├── turtlebot3_waffle_pi
│   │   │   ├── model-1_4.sdf
│   │   │   ├── model.config
│   │   │   └── model.sdf
│   │   └── turtlebot3_world
│   │       ├── meshes
│   │       │   ├── hexagon.dae
│   │       │   └── wall.dae
│   │       ├── model-1_4.sdf
│   │       ├── model.config
│   │       └── model.sdf
│   ├── package.xml
│   ├── rviz
│   │   ├── multi_turtlebot3_slam.rviz
│   │   └── turtlebot3_gazebo_model.rviz
│   ├── src
│   │   └── turtlebot3_drive.cpp
│   └── worlds
│       ├── empty.world
│       ├── turtlebot3_autorace_2020.world
│       ├── turtlebot3_autorace.world
│       ├── turtlebot3_house.world
│       ├── turtlebot3_stage_1.world
│       ├── turtlebot3_stage_2.world
│       ├── turtlebot3_stage_3.world
│       ├── turtlebot3_stage_4.world
│       └── turtlebot3_world.world
└── turtlebot3_simulations
    ├── CHANGELOG.rst
    ├── CMakeLists.txt
    └── package.xml



# MAKE SURE PROJECT MANAGERS UPDATE THIS MD 
