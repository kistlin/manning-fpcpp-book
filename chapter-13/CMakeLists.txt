
add_executable(bookmark-service-testing   bookmark-service-testing/main.cpp)
add_executable(count-lines-test   count-lines-test/main.cpp)
add_executable(count-lines-test-generation   count-lines-test-generation/main.cpp)
add_executable(distances   distances/main.cpp)
target_link_libraries(bookmark-service-testing PRIVATE Catch2WithMain)
target_link_libraries(count-lines-test PRIVATE Catch2WithMain)
target_link_libraries(count-lines-test-generation PRIVATE Catch2WithMain)

set_property(TARGET bookmark-service-testing   PROPERTY FOLDER "examples/chapter-13")
set_property(TARGET count-lines-test   PROPERTY FOLDER "examples/chapter-13")
set_property(TARGET count-lines-test-generation   PROPERTY FOLDER "examples/chapter-13")
set_property(TARGET distances   PROPERTY FOLDER "examples/chapter-13")
