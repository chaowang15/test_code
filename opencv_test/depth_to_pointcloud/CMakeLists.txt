project(depth_to_pointcloud)
add_executable(${PROJECT_NAME} depth_to_pointcloud.cpp)
target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})

set_target_properties(${PROJECT_NAME}
    PROPERTIES
    ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib"
    LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin"
    RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin"
)
