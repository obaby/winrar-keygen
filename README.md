# WinRAR-Keygen

## 1. What is WinRAR?
  * WinRAR is a trialware file archiver utility for Windows, developed by Eugene Roshal of win.rar GmbH. 
  * It can create and view archives in RAR or ZIP file formats and unpack numerous archive file formats. 
  * WinRAR is not a free software. If you want to use it, you should pay to [__RARLAB__](https://rarlab.com/) and then you will get a license file named `"rarreg.key"`. 
  * This repository will tell you how WinRAR license file `"rarreg.key"` is generated. 

## 2. How is "rarreg.key" generated?
  * TODO

## 3. How to build keygen?
  * Please make sure that you have Visual Studio 2015 or the higher. Because this is a VS2015 project.
  * You can open the project by VS2015 IDE and then build it with one click. Or use VS Developer Command Prompt: 
    ```cmd
    msbuild winrar-keygen.vcxproj /p:Configuration=Release;Platform=<x86|x64>;OutputPath=<your_output_dir> /t:build
    ```
  * __NOTICE: Do not use "Debug" configuration. Otherwise you may approximately wait for half a minute every time you generate a license file.__

## 4. Example
    ```cmd
    D:\Github\winrar-keygen>msbuild winrar-keygen.vcxproj /p:Configuration=Release;Platform=x64;OutDir=D:\winrar-keygen\ /t:build
        ......
        ......

    D:\Github\winrar-keygen>cd D:\winrar-keygen

    D:\winrar-keygen>winrar-keygen.exe "Phantom" "Single PC License" >> rarreg.key

    ```