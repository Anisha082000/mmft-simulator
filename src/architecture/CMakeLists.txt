set(SOURCE_LIST
    Channel.hh
    ChannelPosition.hh
    Membrane.hh
    Module.hh
    Network.hh
    Tank.hh
    Edge.hh
    FlowRatePump.hh
    Node.hh
    PressurePump.hh
)
    
set(HEADER_LIST
    Channel.h
    ChannelPosition.h
    Membrane.h
    Module.h
    ModuleOpening.h
    Network.h
    Tank.h
    Edge.h
    FlowRatePump.h
    Node.h
    PressurePump.h
)

target_sources(${TARGET_NAME} PUBLIC ${SOURCE_LIST} ${HEADER_LIST})
target_include_directories(${TARGET_NAME} PUBLIC ${CMAKE_CURRENT_LIST_DIR})
target_link_libraries(${TARGET_NAME} PUBLIC nlohmann_json::nlohmann_json)
