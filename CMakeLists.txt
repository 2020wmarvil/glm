add_subdirectory(glm)

target_include_directories(${ENGINE_NAME} PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(${ENGINE_NAME} PRIVATE glm)
set_target_properties(glm PROPERTIES FOLDER "glm")
#set_property(GLOBAL PROPERTY USE_FOLDERS ON)