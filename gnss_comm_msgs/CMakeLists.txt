cmake_minimum_required(VERSION 3.0.2)
project(gnss_comm_msgs)

find_package(catkin REQUIRED COMPONENTS
  std_msgs
  message_generation
)

add_message_files(FILES 
    GnssTimeMsg.msg
    GnssEphemMsg.msg
    GnssGloEphemMsg.msg
    GnssMeasMsg.msg
    GnssObsMsg.msg
    GnssBestXYZMsg.msg
    GnssPVTSolnMsg.msg
    GnssSvsMsg.msg
    GnssTimePulseInfoMsg.msg
    StampedFloat64Array.msg
)

generate_messages(DEPENDENCIES std_msgs)

catkin_package(CATKIN_DEPENDS std_msgs message_runtime)



