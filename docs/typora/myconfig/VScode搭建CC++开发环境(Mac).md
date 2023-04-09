# VScode搭建C/C++开发环境(Mac)

- vscode安装C/C++插件，codelldb插件

```c++
#include <iostream>
using namespace std;
int main()
{
    cout << "hello hhhh" << endl;
    return 0;
}
```

- Debug，选择添加`launch.json`配置文件，选择LLDB环境

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20201112160153.png" alt="image-20201022144144040" style="zoom: 33%;" />

- 修改成`${fileBasenameNoExtension}`，如果报错找不到该文件，将这个名字改成执行代码的文件名不带后缀。

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20201112160156.png" alt="image-20201022144439932" style="zoom: 33%;" />

- build编译部分。shift+command+p调出控制面板选择Configure Task生成`tasks.json`文件

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20201112160201.png" alt="image-20201022144646347" style="zoom:33%;" />

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20201112160205.png" alt="image-20201022144816332" style="zoom: 33%;" />

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20201112160209.png" alt="image-20201022144935344" style="zoom:33%;" />![image-20201022145131435](https://gitee.com/jellyfive/blog-image/raw/master/image/20201112160213.png)

- 从`tasks.json`的`label`里面复制到`launch.json`的`preLaunchTask`

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20201112160218.png" alt="image-20201022145202444" style="zoom:33%;" />

- F5调试。

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20201112160222.png" alt="image-20201022153137050" style="zoom:33%;" />

