add_subdirectory(glm)
add_library(glm::glm ALIAS glm)
target_include_directories(glm_static PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})

target_include_directories(${ENGINE_NAME} PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(${ENGINE_NAME} PRIVATE glm)