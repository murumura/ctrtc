cmake_minimum_required(VERSION 3.16)

set(project_test

    ${CMAKE_SOURCE_DIR}/test/main.cc
    ${CMAKE_SOURCE_DIR}/test/test_vec.cc
    ${CMAKE_SOURCE_DIR}/test/test_matrix.cc
    ${CMAKE_SOURCE_DIR}/test/test_transform.cc
    ${CMAKE_SOURCE_DIR}/test/test_world.cc
    ${CMAKE_SOURCE_DIR}/test/test_math.cc
    ${CMAKE_SOURCE_DIR}/test/test_ray.cc
    ${CMAKE_SOURCE_DIR}/test/test_canvas.cc
    ${CMAKE_SOURCE_DIR}/test/test_static_vector.cc
    ${CMAKE_SOURCE_DIR}/test/test_intersection.cc
    ${CMAKE_SOURCE_DIR}/test/test_shape.cc
    ${CMAKE_SOURCE_DIR}/test/test_shading.cc
    ${CMAKE_SOURCE_DIR}/test/test_camera.cc
    ${CMAKE_SOURCE_DIR}/test/test_pattern.cc
)

add_executable(raytracer_test
	${project_test}
    ${project_headers}
)
target_compile_options(raytracer_test  PUBLIC  ${COMPILE_DEFINITIONS})
target_include_directories(raytracer_test
    PRIVATE
        ${CMAKE_SOURCE_DIR}/include
)

target_link_libraries(raytracer_test
    gtest
    gtest_main
    pthread
)
