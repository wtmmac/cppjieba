PROJECT(CPPJIEBA)
SET(CMAKE_INSTALL_PREFIX  /usr)
ADD_DEFINITIONS(-std=c++0x -O3)
IF (DEFINED ENC)
    ADD_DEFINITIONS(-DCPPJIEBA_${ENC})
ENDIF()
ADD_SUBDIRECTORY(src)
ADD_SUBDIRECTORY(dicts)
ADD_SUBDIRECTORY(scripts)
ADD_SUBDIRECTORY(conf)
