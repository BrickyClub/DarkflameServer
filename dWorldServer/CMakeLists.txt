set(DWORLDSERVER_SOURCES "ObjectIDManager.cpp"
		"PerformanceManager.cpp"
		"WorldServer.cpp")

add_executable(WorldServer ${DWORLDSERVER_SOURCES})
target_link_libraries(WorldServer ${COMMON_LIBRARIES} dChatFilter dGame dZoneManager Detour Recast dPhysics tinyxml2 dNavigation)
