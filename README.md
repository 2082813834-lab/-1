# my_cpp_project

示例 C++ 项目（CMake）。

构建（在项目根目录）：
mkdir -p build
cd build
cmake ..
cmake --build . --config Release

在 Windows 上如果使用 MinGW，你可能先用:
cmake -G "MinGW Makefiles" ..
mingw32-make

运行：
# 在 build 目录下
./my_app    # 或 my_app.exe (Windows)
