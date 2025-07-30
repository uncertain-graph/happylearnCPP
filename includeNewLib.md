# Include External library

## Visual Studio Community
+ Project > Properties > Configuration Properties > C/C++ > General 
+ Additional Include Directiories 添加Eigen 库的路径
+ 在main.cpp文件中添加Eigen库的头文件
+ 构建编译并运行

## Clion 
+ 打开Clion并加载项目
+ 在项目的根目录下，打开`CMakeLists.txt`文件
+ 在文件中添加以下内容
  ```
  set(EIGEN3_INCLUDE_DIR "C:/Libraries/eigen-3.4.0")
  include_directories(${EIGEN3_INCLUDE_DIR})
  # 或者你也可以使用 find_package 来自动找到 Eigen
  # find_package(Eigen3 3.3 REQUIRED NO_MODULE)
  ```
+ CLion会自动检测和加载CMake配置，在修改文件之后，CLion会自动重新加载项目，确保新的头文件路径被正确识别
+ 在main.cpp文件中添加Eigen库的头文件
