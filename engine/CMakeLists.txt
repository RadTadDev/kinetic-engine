add_library(Kinetic STATIC
    "src/Application.cpp"
 )

target_include_directories(Kinetic PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)


find_package(SDL3 CONFIG REQUIRED)
target_link_libraries(Kinetic PUBLIC SDL3::SDL3)