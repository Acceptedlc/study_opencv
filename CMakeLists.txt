 project( opencv_study )
 set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)

 find_package( OpenCV REQUIRED )

 add_executable( displayImage ${CMAKE_CURRENT_SOURCE_DIR}/src/display_image_01.cc)
 target_link_libraries( displayImage ${OpenCV_LIBS} )