project(sb7exercise)
cmake_minimum_required(VERSION 2.8)
add_definitions(-D__gl_h_ -DGL_DO_NOT_WARN_IF_MULTI_GL_VERSION_HEADERS_INCLUDED -D_DEBUG)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -framework CoreFoundation")
# chapter2
## first app
set(FIRST_APP_SRC chapter2/first_app/main.cpp)
add_executable(first_app ${FIRST_APP_SRC})
target_link_libraries(first_app -lsb7 -lglfw3 -lgl3w)
## first shader
set(FIRST_SHADER_SRC chapter2/first_shader/shader_loader.cpp chapter2/first_shader/main.cpp)
add_executable(first_shader ${FIRST_SHADER_SRC})
target_link_libraries(first_shader -lsb7 -lglfw3 -lgl3w)
## first triangle
set(FIRST_TRIANGLE_SRC chapter2/first_triangle/shader_loader.cpp chapter2/first_triangle/main.cpp)
add_executable(first_triangle ${FIRST_TRIANGLE_SRC})
target_link_libraries(first_triangle -lsb7 -lglfw3 -lgl3w)

# chapter3
## update vertex attribute
set(UPDATE_VERTEX_ATTRIBUTE_SRC chapter3/update_vertex_attribute/shader_loader.cpp chapter3/update_vertex_attribute/main.cpp)
add_executable(update_vertex_attribute ${UPDATE_VERTEX_ATTRIBUTE_SRC})
target_link_libraries(update_vertex_attribute -lsb7 -lglfw3 -lgl3w)
## different colored triangle
set(DIFFERENT_COLORED_TRIANGLE_SRC chapter3/different_colored_triangle/shader_loader.cpp chapter3/different_colored_triangle/main.cpp)
add_executable(different_colored_triangle ${DIFFERENT_COLORED_TRIANGLE_SRC})
target_link_libraries(different_colored_triangle -lsb7 -lglfw3 -lgl3w)
## interface block triangle
set(INTERFACE_BLOCK_TRIANGLE_SRC chapter3/interface_block_triangle/shader_loader.cpp chapter3/interface_block_triangle/main.cpp)
add_executable(interface_block_triangle ${INTERFACE_BLOCK_TRIANGLE_SRC})
target_link_libraries(interface_block_triangle -lsb7 -lglfw3 -lgl3w)
## triangle with tessellation
set(TRIANGLE_WITH_TESSELLATION_SRC chapter3/triangle_with_tessellation/shader_loader.cpp chapter3/triangle_with_tessellation/main.cpp)
add_executable(triangle_with_tessellation ${TRIANGLE_WITH_TESSELLATION_SRC})
target_link_libraries(triangle_with_tessellation -lsb7 -lglfw3 -lgl3w)
## triangle with tessellation and geometry shader
set(TRIANGLE_WITH_TESS_GEOMETRY_SRC chapter3/triangle_with_tess_geometry/shader_loader.cpp chapter3/triangle_with_tess_geometry/main.cpp)
add_executable(triangle_with_tess_geometry ${TRIANGLE_WITH_TESS_GEOMETRY_SRC})
target_link_libraries(triangle_with_tess_geometry -lsb7 -lglfw3 -lgl3w)
## triangle with fragment shader
set(TRIANGLE_WITH_FRAGSHADER_SRC chapter3/triangle_with_fragshader/shader_loader.cpp chapter3/triangle_with_fragshader/main.cpp)
add_executable(triangle_with_fragshader ${TRIANGLE_WITH_FRAGSHADER_SRC})
target_link_libraries(triangle_with_fragshader -lsb7 -lglfw3 -lgl3w)
## triangle color smooth
set(TRIANGLE_COLOR_SMOOTH_SRC chapter3/triangle_color_smooth/shader_loader.cpp chapter3/triangle_color_smooth/main.cpp)
add_executable(triangle_color_smooth ${TRIANGLE_COLOR_SMOOTH_SRC})
target_link_libraries(triangle_color_smooth -lsb7 -lglfw3 -lgl3w)
