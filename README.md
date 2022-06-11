### CppAD ipopt简介:
- Ipopt (Interior Point OPTimizer, pronounced eye-pea-Opt) is a software package for large-scale nonlinear optimization。Ipopt是一个大规模非线性连续优化的软件包，使用C++实现。
- CppAD: A tool for differentiation of C++ functions。CppAD是一个微分工具包，使用C++实现，同时CppAD需要依赖系统中已经安装好的优化求解器，如Ipopt

- 安装CppAD
```
sudo apt-get install cppad
```
- 安装Ipopt
```
https://zhuanlan.zhihu.com/p/389375147
```

### CMakeLists.txt
 - set(sources src/ipopt_test.cpp)指定源文件
 - include_directories(src/Eigen-3.3)指定Eigen矩阵库
 
 
### 编译
```
mkdir build
cd build
cmake ..
make -j4
```


### 运行
```
./ipopt_test
```
