set(SOURCES
  LDDProfilingRuntime.cpp
  TimerProfilingRuntime.cpp
  )

add_llvm_library( LDDProfilingRuntime-static ${SOURCES} )
set_target_properties( LDDProfilingRuntime-static
  PROPERTIES
  OUTPUT_NAME "LDDProfilingRuntime" )

set(BUILD_SHARED_LIBS ON)
add_llvm_library( LDDProfilingRuntime-shared ${SOURCES} )
set_target_properties( LDDProfilingRuntime-shared
  PROPERTIES
  OUTPUT_NAME "LDDProfilingRuntime" )
