![](/assets/Screen Shot 2018-02-27 at 11.31.59.png)

> 官网官网提示，上传代码模块也可使用twine，本文将使用twine上传。

## 1.准备工作

安装twine，后续操作将通过twine上传模块

```
pip install twine
```

编写代码模块，新建shuxcTestPyPI.py测试文件，准备将此代码上传至PyPI

```
def printPyPI():
  print("this is my first PyPI!")
```

新建新建setup.py 文件（与shuxcTestPyPI.py同目录）。配置模块相关信息

```
from distutils.core import setup

setup(
    name='shuxcTestPyPI',
    version='1.0.0',
    packages=[''],
    url=' ',
    license='',
    author='smicro',
    author_email='shuxc_dev@163.com',
    description='My Test'
)
```

## 2.检测配置文件\(可跳过\)

```
Python setup.py check
```

出现running check则表示正常

## 3.生成dist目录

```
Python setup.py sdist
```

在文件目录下出现一个dist文件夹以及MANIFEST文件，截图如下：![](/assets/Screen Shot 2018-02-27 at 11.18.59.png)

## 4.使用twine 上传模块

```
twine upload dist/*
```

> 本人在此处出现“400 Client Error: User 'smicro' has no verified email addresses...”，提示未验证邮箱。
>
> 验证邮箱后重新上传成功
>
> ![](/assets/Screen Shot 2018-02-27 at 11.22.06.png)

## 5.登陆官查看上传的模块

![](/assets/Screen Shot 2018-02-27 at 11.32.22.png)

