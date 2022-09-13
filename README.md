# EPANET Build
https://github.com/OpenWaterAnalytics/EPANET.git

## build script
```
$ git clone https://github.com/OpenWaterAnalytics/EPANET.git
$ cd .\EPANET\
$ mkdir build
$ cd .\build\
$ cmake ..

## error 확인
$ ii .\CMakeFiles\CMakeOutput.log
$ ii .\CMakeFiles\CMakeError.log

## 다시 빌드
$ cmake ..
$ cmake --build . --config Release
$ ls .\bin\Release\epanet2.dll
```

## build error
1. MSB8003
1) 원인
https://docs.microsoft.com/ko-kr/visualstudio/msbuild/errors/msb8003?view=vs-2022
 C/C++ 도구 집합을 설치가 안되어있어서 원인 발생

2) 해결
https://docs.microsoft.com/ko-kr/visualstudio/install/modify-visual-studio?view=vs-2022
도구-> Desktop에 필요한 개발도구들 설치

## Reference
https://github.com/OpenWaterAnalytics/EPANET/blob/master/BUILDING.md
