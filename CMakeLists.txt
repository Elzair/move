cmake_minimum_required(VERSION 3.3)

project(boost_move)

add_library(boost_move INTERFACE)

target_include_directories(boost_move BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_move DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
