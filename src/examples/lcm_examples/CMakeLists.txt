PIXHAWK_EXECUTABLE(lcmsend lcmsend.cc)
PIXHAWK_LINK_LIBRARIES(lcmsend
  lcmext
  ${Boost_PROGRAM_OPTIONS_LIBRARY}
)

PIXHAWK_EXECUTABLE(lcmreceive lcmreceive.cc)
PIXHAWK_LINK_LIBRARIES(lcmreceive
  lcmext
  ${Boost_PROGRAM_OPTIONS_LIBRARY}
  ${GTHREAD2_LIBRARY}
)
