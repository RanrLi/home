PROJECT(lrr-5)

FILE(GLOB lrr-5_SRCS
    devil.hpp
    devil.cpp
    main.cpp
    Task.h
    Task.cpp
    Sort.h
    Sort.cpp
    Robot.h
    Robot.cpp
    InfoCons.h
    InfoCons.cpp
    class.h
    readyadvence.h
    readyadvence.cpp
    two_table.h
	planwithtask.cpp
	action.cpp
)
SOURCE_GROUP("" FILES ${lrr-5_SRCS})

ADD_EXECUTABLE(lrr-5 ${lrr-5_SRCS})

ADD_DEPENDENCIES(lrr-5 frame utility)
TARGET_LINK_LIBRARIES(lrr-5 frame utility ${Boost_LIBRARIES})
