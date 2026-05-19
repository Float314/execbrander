cmake_minimum_required(VERSION 3.15)

project(example)

include(../src/execbrander.cmake)

# Set the path to the JSON file
set(json_path "${CMAKE_CURRENT_SOURCE_DIR}/../src/example.json")
# Call the function to generate the metadata.rc file
execbrand_embedrc(${PROJECT_NAME} "${json_path}")

add_executable(example main.cpp "${CMAKE_CURRENT_BINARY_DIR}/metadata.rc")