set(COMPONENT_NAME propertyeditor)

set(SRC
    propertyeditordialog.ui
    propertyeditordialog.cpp
)

add_library(${COMPONENT_NAME} ${SRC})
include_directories("${CMAKE_CURRENT_SOURCE_DIR}/..")
target_link_libraries(${COMPONENT_NAME} Qt5::Widgets Qt5::Core cds-common)
target_include_directories(${COMPONENT_NAME} INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})


