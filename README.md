#### Question:
  QtCreator 12.0.1 can not support Conan 2.0.9, this repo is for finding errors.

#### Reproduce by install Qt6 on Windows11
1. Qt 6.6.1
2. QtCreator 12.0.1
3. VS 2022
4. conan 2.0.9
5. cmake 3.27.7

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
