PROJECT(githublbp)
SET(CMAKE_BUILD_TYPE Release)
CMAKE_MINIMUM_REQUIRED( VERSION 2.6 )
FIND_PACKAGE( OpenCV REQUIRED )
ADD_EXECUTABLE(imagelbp imagelbp.cpp lbp.cpp histogram.cpp)
TARGET_LINK_LIBRARIES(imagelbp ${OpenCV_LIBS})
