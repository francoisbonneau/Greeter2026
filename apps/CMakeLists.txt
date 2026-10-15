#add the executable target named greet
add_executable(greet greet.cpp)

# add binary tree to the list of paths to search includes
target_include_directories(greet PUBLIC "${PROJECT_BINARY_DIR}")
install(TARGETS greet DESTINATION bin)
