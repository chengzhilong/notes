### make ###
1. make用来执行Makefile文件的
2. Makefile是类UNIX环境下的类似于批处理的“脚本”文件。其基本语法是：目标+依赖+命令，只有在目标文件不存在，或目标比依赖的文件更旧，命令才会被执行
3. Makefile+make可理解为类UNIX环境下的项目管理工具，但它太基础了而且抽象程度不高，且对windows不太友好。因此就有了跨平台项目管理工具cmake

### CMake ###
1. cmake是跨平台项目管理工具，使用更抽象的语法来组织项目。虽然，仍然是目标、依赖之类的东西，但更为抽象和友好。比如你可以用math表示数学库，而不需要再具体指定到底是math.dll还是libmath.so，在windows下它会支持生成visual studio的工程，在linux下它会生成makefile，甚至还能生成eclipse工程文件。
2. cmake是抽象层次更高的项目管理工具，cmake命令执行的是CMakeLists.txt文件
3. 下图，cl表示visual studio的编辑器，gcc表示linux下的编辑器![make](https://github.com/chengzhilong/Img/blob/master/picture/make_cmp.png)
