# The 'testrender' executable
FILE(GLOB testrender_src *.cpp)
ADD_EXECUTABLE ( testrender ${testrender_src} )
TARGET_LINK_LIBRARIES ( testrender oslexec oslquery ${OPENIMAGEIO_LIBRARIES} ${Boost_LIBRARIES} ${CMAKE_DL_LIBS})
INSTALL ( TARGETS testrender RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR} )
