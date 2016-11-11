# gtest part
add_subdirectory(gtest)

add_executable(test_gtest test.cpp)
target_link_libraries(test_gtest pthread gtest gtest_main)
add_test(test_gtest ${CMAKE_RUNTIME_OUTPUT_DIRECTORY}/test_gtest)
