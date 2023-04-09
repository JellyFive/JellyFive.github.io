# Endnote文献管理工具

> 本文示例: Mac+Endnote20

## Endnote相关

### 软件安装/新建库

嗯...就百度搜一下叭。

安装完之后要注册一个账户。

首先是新建一个数据库文件：`File-new-...`。win类似。

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20210413172129.png" style="zoom:50%;" />

**若是已有库，或是导入别人的库，直接：`File-Open Library-xxx.enl `**

### 文献导入方法

#### 直接检索

`Tools-Online Search`，选择自己要检索的数据库，这里以Web of sciences为例

![](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413173157.png)

#### xx学术等地方外部导入

1. 先下载好自己的文献
   - 微软学术导出为RIS格式；(.ris)
   - 百度学术导出为Endnote格式；(.enw)
   - 知网导出为Endnote格式...(.txt)

2. `File-import`。大部分时候导入的不成功都是没有找到“option”按钮！

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20210413175150.png" style="zoom:50%;" />

其中，RIS格式文件选择（RIS）

3. 导入成功即为：

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20210413175254.png" style="zoom:33%;" />

#### 插件导入

对于一些检索不到的，可以采用网页检索，插件导入的方式（谷歌）。需要endnote账户登录，用于同步。

1. 下载链接：<https://kopernio.com/endnote?utm_source=endnote&utm_medium=web&utm_campaign=kopernio_clarivate_main_page_tile&ref=endnote>

<img src="https://gitee.com/jellyfive/blog-image/raw/master/image/20210413180028.png" style="zoom:33%;" />)

2. 打开web of science(其他数据库同样适用)，右下角弹出的“查看PDF”。等待论文加载后需要Push到endnote。

![](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413193042.png)

3. 上一步是Push到了web端的endnote。需要本地同步一下。

![](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413200541.png)

至此，本地文献数据库导入完成。

## word中插入文献

这里以中文常用学术论文参考文献格式为例。

### 引用文献格式

1. 常用中文学术论文格式为GB/T7714，endnote本身不带有这个库，需要去官网下载。

[GBT7714格式文件](https://www.endnote.com/downloads/styles/?wpv_post_search=chinese&wpv-citation_style=superscripted-number&wpv_aux_current_post_id=12829&wpv_view_count=12764-TCPID12829)

![](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413201308.png)

2. 下载后可以自己拖到Endnote的样式文件夹。

Mac用户在应用程序里面找到Endnote，进去“Styles”文件夹，把刚刚下载的.ens文件拖进去即可。

Win用户邮件Endnote到文件所在位置......

![](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413201553.png)

3. 在Endnote导入样式文件。win用户在“Output Styles”选项可能不在“Tools”里面，找一找叭。然后“Open Style Manager”，勾选刚刚添加的“Chinese Std ...”。此时标准的参考文献格式已经可以生成。

![](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413201751.png)

4. 在Word中插入参考文献。
   - 打开Word后会出现Endnote20选项卡。在Style中选择刚刚导入的格式文件。
   - 在最左边的Insert Citation中插入参考文献。有两种方式：搜索论文插入（Insert Citation...）；在Endnote中选中待引用文献然后插入（Insert Selected Citation）
   - Configure Bib...中可以修改插入参考文献的格式（间距 字体等）
   - 每次Endnote库更新了格式文件，都要“Update Citations and ...”

![](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413202646.png)

![](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413203437.png)

### 自定义参考文献格式。

给出的文献格式不满足要求，一般可以在基础上进行修改。打开“Output Style选项卡”，选择“Edit xxxx(选中的格式)”，这里会出现一个copy。详细说明如下：

1. 选择期刊名是否缩写。第一个是全称，后面是缩写。

![image-20210413203849036](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413203849.png)

2. 若是选择缩写，则需要导入缩写格式文件。按照下图方式导入，在Endnote的文件路径下找"Terms"文件夹，选择自己领域的缩写文件。

![image-20210413204444485](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413204444.png)

3. 修改引用的上下标。在“Templates”中修改“Citation”。关于文字是否加粗、倾斜、上下标等，在修改的同时选择Edit-Font进行相应的调整。

![image-20210413204639763](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413204639.png)

4. 修改参考文献样式。

   按照自己的格式对Template进行修改，语法百度叭。后面的选项卡可以自行进行调整。

![image-20210413204932016](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413204932.png)

5. 修改之后在wrod中修改Style。然后Update一下，新的参考文献如下：

![image-20210413205349638](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413205349.png)

6. 每一次在word中删除文献，在endnote中修改文献等，都要update一下，会自动更新。

### 分页插入参考文献

对于有的论文要求每一小节参考文献从头开始编号，可以进行如下操作。

#### 对于word

在需要分节的地方，引入分节符。布局-分隔符-分节符-下一页...

#### 对于endnote

对Style文件的Sections部分进行如下修改。

![image-20210413205741824](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413205741.png)

#### 示例

![image-20210413210542974](https://gitee.com/jellyfive/blog-image/raw/master/image/20210413210543.png)

over!