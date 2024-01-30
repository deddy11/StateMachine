cmake_minimum_required(VERSION 3.14)

project(statemachine)

# set(CMAKE_BUILD_TYPE "Debug")

file(GLOB COBA_STATEMACHINE_SRC
    src/*.cpp
	StateMachine/*.cpp
)

add_executable(${PROJECT_NAME} ${COBA_STATEMACHINE_SRC})

target_include_directories(${PROJECT_NAME} PRIVATE
	StateMachine
)

# target_link_libraries(${PROJECT_NAME} PUBLIC
# 	rdkafka
# )