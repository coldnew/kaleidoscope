
include_directories(
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${CMAKE_CURRENT_BUILD_DIR}
  )


set(SOURCE
  main.cpp
  )

ADD_EXECUTABLE(kaleidoscope ${SOURCE})
TARGET_LINK_LIBRARIES(kaleidoscope)

install(
  TARGETS kaleidoscope
  RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR})