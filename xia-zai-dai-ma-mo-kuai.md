![](/assets/Screen Shot 2018-02-27 at 14.29.39.png)

> 官网提示，下载代码模块，通过pip安装，本文以shuxcTestPyPI为例进行下载安装

## 1.下载模块

在在官网上下载shuxcTestPyPI代码模块，下载文件为：shuxcTestPyPI-1.0.0.tar.gz

![](/assets/Screen Shot 2018-02-27 at 14.22.29.png)

## 2.解压模块

解压该文件

```
tar -xzvf shuxcTestPyPI-1.0.0.tar.gz
```

解压后文件结构如下

## ![](/assets/Screen Shot 2018-02-27 at 14.43.35.png)3.build模块

```
python setup.py build
```

build后文件目录如下

## ![](/assets/Screen Shot 2018-02-27 at 14.23.16.png)4.安装模块

```
python setup.py install
```

## ![](/assets/Screen Shot 2018-02-27 at 14.48.11.png)5.使用模块

新建test\_PyPI\_function.py文件，文件内容为

```
import shuxcTestPyPI

shuxcTestPyPI.printHello();
```

 运行此文件

```
python test_PyPI_function.py
```

![](/assets/Screen Shot 2018-02-27 at 14.51.38.png)模块可正常使用

