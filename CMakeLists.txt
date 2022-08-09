cmake_minimum_required(VERSION 3.13)

project(vision)
set(CMAKE_CXX_STANDARD 11)            # Enable c++11 standard

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )

add_executable(capture_images capture_images.cpp) 
target_link_libraries( capture_images ${OpenCV_LIBS} )

add_executable(ball_locator_v1 ball_locator_v1.cpp) 
target_link_libraries( ball_locator_v1 ${OpenCV_LIBS} )

add_executable(play_video play_video.cpp) 
target_link_libraries( play_video ${OpenCV_LIBS} )

#add_executable(hough_lines hough_lines.cpp) 
#target_link_libraries( hough_lines ${OpenCV_LIBS} )

add_executable(canny canny_edge.cpp) 
target_link_libraries( canny ${OpenCV_LIBS} )

add_executable(canny_tst canny_tst.cpp) 
target_link_libraries( canny_tst ${OpenCV_LIBS} )

#dd_executable(hough_slider hough_trackbar.cpp) 
#target_link_libraries( hough_slider ${OpenCV_LIBS} )

#add_executable(hsv_threshold hsv_threshold.cpp) 
#target_link_libraries( hsv_threshold ${OpenCV_LIBS} )

add_executable(opt_flow opt_flow.cpp) 
target_link_libraries( opt_flow ${OpenCV_LIBS} )
