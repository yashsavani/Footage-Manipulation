# Create exectuable with target name "calibrate"
add_executable(calibrate calibrate.cpp)
add_executable(undistort undistort.cpp)
add_executable(stabilize stabilize.cpp)
add_executable(split_vid split_vid.cpp)

# Link target with libraries
target_link_libraries(calibrate ${OpenCV_LIBS} ${Boost_LIBRARIES})
target_link_libraries(undistort ${OpenCV_LIBS} ${Boost_LIBRARIES})
target_link_libraries(stabilize ${OpenCV_LIBS} ${Boost_LIBRARIES})
target_link_libraries(split_vid ${OpenCV_LIBS} ${Boost_LIBRARIES})
