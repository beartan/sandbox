cmake_minimum_required(VERSION 2.6)
 
PROJECT(RenderWindow)
 
FIND_PACKAGE(VTK)
INCLUDE(${VTK_USE_FILE})
 
FIND_PACKAGE(Qt4 REQUIRED)
INCLUDE(${QT_USE_FILE})
 
ADD_EXECUTABLE(RenderWindow renderwindow.cxx)
TARGET_LINK_LIBRARIES(RenderWindow QVTK vtkHybrid)
