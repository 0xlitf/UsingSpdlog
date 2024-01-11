### Question:
  QtCreator 12.0.1 can not support Conan 2.0.9, this repo is for finding errors.
  
1. [https://github.com/conan-io/cmake-conan/issues/608](https://github.com/conan-io/cmake-conan/issues/608)
  
2. [https://forum.qt.io/topic/153573/conan-install-error-on-qtcreator-12-0-0-12-0-1/6](https://forum.qt.io/topic/153573/conan-install-error-on-qtcreator-12-0-0-12-0-1/6)


### Interim solution
1. Replace `C:\Qt\Tools\QtCreator\share\qtcreator\package-manager\auto-setup.cmake` with [auto-setup.cmake](https://code.qt.io/cgit/qt-creator/qt-creator.git/tree/src/share/3rdparty/package-manager/auto-setup.cmake?h=12.0)
2. Manually specify `CMAKE_MSVC_RUNTIME_LIBRARY` in [CMakeLists.txt](https://github.com/0xlitf/UsingSpdlog/blob/main/CMakeLists.txt)

  
### memsharded closed this as completed:
1. [https://github.com/conan-io/cmake-conan/issues/608](https://github.com/conan-io/cmake-conan/issues/608)
2. [https://github.com/conan-io/cmake-conan/pull/609](https://github.com/conan-io/cmake-conan/pull/609)
   
Thanks to [James](https://github.com/memsharded), [Cristian Adam](https://github.com/cristianadam).


### Reproduce by install Qt6 on Windows11
1. Qt 6.6.1
2. QtCreator 12.0.1
3. VS 2022
4. conan 2.0.9
5. cmake 3.27.7
