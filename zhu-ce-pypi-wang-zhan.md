> 如下介绍了两种注册PyPI网站方式。第一种直接登陆官网注册，第二种通过命令注册。

## 1.登陆官网注册

登陆PyPI官网（_https://pypi.org/_）注册，本人注册时一直提示“Recaptcha error”，留个截图，以后再验证。

![](/assets/Screen Shot 2018-02-27 at 09.59.40.png)

## 2.命令注册

新建一个setup.py文件

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

在同目录下运行命令：

`python setup.py register`

![](/assets/Screen Shot 2018-02-27 at 10.17.58.png)选择 2 根据提示填写账号，密码（密码需大小写字母，特殊符），邮箱，验证邮箱收到的链接完成注册。





