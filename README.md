# VScode-CPP_envpacket-EZdeploy
资源来自B站UP：SDchao  https://github.com/SDchao/AutoVsCEnv_WPF/issues/new
## 一、打开AutoVsCEnv_WPF.exe，选择MinGW安装地址，选择日后存放源代码的地址，自动在线下载MinGW后，自行打开VScode，自动安装依赖。  
## 二、安装完毕后，运行之前选定文件夹中的test.c测试安装结果，此时VScode能正常编译运行c++程序，但字符集没有正确配置，可能会导致中文乱码的情况。  
### 将head.h文件放在.vscode文件夹下，并对该目录下task.jason进行修改  
- 整行替换："args": ["-m32","-g", "'${file}'","-include","${workspaceRoot}/.vscode/head.h", "-o", "'${fileDirname}/${fileBasenameNoExtension}.exe'"]
