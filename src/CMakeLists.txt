enable_testing()

add_executable(
    example_test
    example_test.cpp)
target_link_libraries(
    example_test
     gtest_main)

add_test(
    NAME example_test
    COMMAND example_test
)

include(GoogleTest)
gtest_discover_tests(example_test)



