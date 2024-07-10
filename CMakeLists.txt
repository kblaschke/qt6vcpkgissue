cmake_minimum_required(VERSION 3.25)

project(Qt6IssueWithVcpkg
        LANGUAGES C CXX
)

find_package(Qt6 REQUIRED COMPONENTS Core)

add_executable(test main.cpp)

target_link_libraries(test
        PRIVATE
        Qt6::Core
)

