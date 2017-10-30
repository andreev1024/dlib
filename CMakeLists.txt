cmake_minimum_required(VERSION 2.8.12)
# Every project needs a name.
project(facedetect)

# Tell cmake we will need dlib.  This command will pull in dlib and compile it
# into your project.  Note that you don't need to compile or install dlib.  All
# it needs is the dlib source code folder and it will take care of everything.
include(/home/andreev/www/dlib-prod/dlib/cmake)

add_executable(facedetect facedetect.cpp)
target_link_libraries(facedetect dlib::dlib )


