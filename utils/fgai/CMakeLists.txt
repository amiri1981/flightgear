add_executable(fgai
  fgai.cxx
  HLAAircraft.cxx
  HLAAircraftClass.cxx
  HLAAirVehicle.cxx
  HLAAirVehicleClass.cxx
  AIBVHPager.cxx
  AIEnvironment.cxx
  AIManager.cxx
  AIObject.cxx
  AIPhysics.cxx
  HLABaloon.cxx
  HLABaloonClass.cxx
  HLAMPAircraft.cxx
  HLAMPAircraftClass.cxx
  HLASceneObject.cxx
  HLASceneObjectClass.cxx
)

target_link_libraries(fgai
  ${SIMGEAR_LIBRARIES}
  ${OPENSCENEGRAPH_LIBRARIES}
  ${OPENGL_LIBRARIES}
  ${RTI_LIBRARIES}
  ${SIMGEAR_CORE_LIBRARY_DEPENDENCIES}
)

install(TARGETS fgai RUNTIME DESTINATION bin)
