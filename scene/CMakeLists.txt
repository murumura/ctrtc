if ((${RENDER_CHAPTER} STREQUAL 4))
    add_executable(CHAPTER4
        ${project_headers}
        clock.cc
    )
    target_compile_options(CHAPTER4  PUBLIC  ${COMPILE_DEFINITIONS})
endif()

if ((${RENDER_CHAPTER} STREQUAL 5))
    add_executable(CHAPTER5
        ${project_headers}
        sphere_on_wall.cc
    )
    target_compile_options(CHAPTER5  PUBLIC  ${COMPILE_DEFINITIONS})
endif()

if ((${RENDER_CHAPTER} STREQUAL 6))
    add_executable(CHAPTER6
        ${project_headers}
        silhouette_sphere.cc
    )
    target_compile_options(CHAPTER6  PUBLIC  ${COMPILE_DEFINITIONS})
endif()


if ((${RENDER_CHAPTER} STREQUAL 7))
    add_executable(CHAPTER7
        ${project_headers}
        scene.cc
    )
    target_compile_options(CHAPTER7  PUBLIC  ${COMPILE_DEFINITIONS})
endif()


if ((${RENDER_CHAPTER} STREQUAL 8))
    add_executable(CHAPTER8
        ${project_headers}
        scene.cc
    )
    target_compile_options(CHAPTER8  PUBLIC  ${COMPILE_DEFINITIONS})
endif()


if ((${RENDER_CHAPTER} STREQUAL 9))
    add_executable(CHAPTER9
        ${project_headers}
        plane.cc
    )
    target_compile_options(CHAPTER9  PUBLIC  ${COMPILE_DEFINITIONS})
endif()

if ((${RENDER_CHAPTER} STREQUAL 10))
    add_executable(CHAPTER10
        ${project_headers}
        pattern.cc
    )
    target_compile_options(CHAPTER10  PUBLIC  ${COMPILE_DEFINITIONS})
endif()
