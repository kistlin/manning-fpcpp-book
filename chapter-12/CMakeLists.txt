SET(SOURCES_BOOKMARK_SERVICE
        bookmark-service/main.cpp
        bookmark-service/service.cpp
)

SET(SOURCES_BOOKMARK_SERVICE_WITH_REPLY
        bookmark-service-with-reply/main.cpp
        bookmark-service-with-reply/service.cpp
)

add_executable(bookmark-service  ${SOURCES_BOOKMARK_SERVICE})
add_executable(bookmark-service-with-reply ${SOURCES_BOOKMARK_SERVICE_WITH_REPLY})
target_include_directories(bookmark-service PRIVATE ${Boost_INCLUDE_DIRS})

set_property(TARGET bookmark-service   PROPERTY FOLDER "examples/chapter-12")
set_property(TARGET bookmark-service-with-reply   PROPERTY FOLDER "examples/chapter-12")
