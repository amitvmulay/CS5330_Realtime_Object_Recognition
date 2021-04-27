cmake_minimum_required(VERSION 3.15)

project(CVProject2)

# Include headers
include_directories("/usr/local/include/")
include_directories("./include/")

set(CMAKE_BUILD_TYPE Debug)
# Create the executable
#file(GLOB SRC "src/*.cpp")
add_executable(cbirgui ./src/main.cpp ./src/DataBase.cpp)

find_package(OpenCV REQUIRED)
target_link_libraries(Project3 ${OpenCV_LIBS})
#target_link_libraries(baseLineMatching ${OpenCV_LIBS})



