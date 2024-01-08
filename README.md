### QtCreator 12.0.0/12.0.1 can not support Conan 2.0.9, this repo is for finding errors.

### Reproduce by install Qt6 on Windows11, installer of Qt6 [qt-creator-opensource-windows-x86_64-11.0.3.exe](https://qt.mirror.constant.com/official_releases/qtcreator/11.0/11.0.3/qt-creator-opensource-windows-x86_64-11.0.3.exe)
### Qt 6.6.1 + QtCreator 12.0.1 + conan 2.0.9 (or conan 2.0.16, with same error)


### my profile of conan2:
C:\Users\QtDev\\.conan2\profiles\default:
```
[settings]
arch=x86_64
build_type=Release
compiler=msvc
compiler.cppstd=14
compiler.runtime=dynamic
compiler.version=193
os=Windows
[options]
shared=True
```
