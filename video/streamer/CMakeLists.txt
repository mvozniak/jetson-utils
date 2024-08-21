
file(GLOB videoViewerSources *.cpp)
file(GLOB videoViewerIncludes *.h )

add_executable(streamer ${videoViewerSources})
target_link_libraries(streamer jetson-utils)

install(TARGETS streamer DESTINATION bin)
