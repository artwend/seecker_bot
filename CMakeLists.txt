cmake_minimum_required(VERSION 3.17)
project(seecker_bot)

set(CMAKE_CXX_STANDARD 20)

add_executable(seecker_bot main.cpp)

find_package(OpenCV CONFIG REQUIRED)
find_package(PThreads_windows CONFIG REQUIRED)

target_link_libraries(seecker_bot PRIVATE
        PThreads_windows::PThreads_windows
        ${OpenCV_LIBS} opencv_ml opencv_dnn opencv_core opencv_flann
        )