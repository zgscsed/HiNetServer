# 使用该文件cmake支持的最低版本
cmake_minimum_required(VERSION 3.5)

# 生成的可执行项目名称
project(Hinet)
# 创建变量，c++版本
set(CMAKE_CXX_STANDARD 11)

#设置可执行目标文件的输出目录
SET(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/build/debug) 
# 源文件， 设置变量，创建变量来代替要进行编译的文件。
# 在CMake中，变量的使用好像都是 ${变量名} 这种格式。
set(SOURCE_FILES
    src/main.cpp
)

# 使用指定的源文件来生成目标可执行文件
add_executable(Hinet ${SOURCE_FILES})