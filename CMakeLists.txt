file(GLOB SOURCE_FILES "src/*.cpp")

add_library(yaml-cpp "${SOURCE_FILES}")
target_compile_features(yaml-cpp PRIVATE cxx_std_11)
target_include_directories(yaml-cpp PUBLIC include src)