add_executable(live555MediaServer
    DynamicRTSPServer.cpp
    DynamicRTSPServer.hh
    live555MediaServer.cpp
    version.hh
)
target_link_libraries(live555MediaServer PRIVATE
    live555_cxx_flags
    liveMedia
    BasicUsageEnvironment
)
set_target_properties(live555MediaServer PROPERTIES FOLDER "Live555/Servers")
