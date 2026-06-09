cmake_minimum_required(VERSION 3.0.2)
project(indooruav_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_generation
)

add_service_files(
  FILES
    CameraVideoConfig.srv
    CameraZoom.srv
    GimbalAngle.srv
    GimbalYawFollow.srv
    TransferMissionMedia.srv
    UploadImageBytes.srv
    UavCameraSetVideoResolution.srv
    UavCameraShoot.srv
    UavCameraVideoEnd.srv
    UavCameraVideoStart.srv
    UavCameraZoomFactor.srv
    UavGimbalPitchAngle.srv
    UavLand.srv
    UavTakeoff.srv
)

generate_messages()

catkin_package(
  CATKIN_DEPENDS message_runtime
)
