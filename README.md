安装 virtualenvwrapper ：

1. linux系统

pip install virtualenvwrapper
2. windows系统

pip install virtualenvwrapper-win
1. 创建虚拟环境

mkvirtualenv my_env
那么会在你当前用户下创建一个 Env 的文件夹，然后将这个虚拟环境安装到这个目录下。

如果你电脑中安装了 python2 和 python3 ，并且两个版本中都安装了 virtualenvwrapper ，
那么将会使用环境变量中第一个出现的 Python 版本来作为这个虚拟环境的 Python 解释器。

2. 切换到某个虚拟环境

workon my_env
3. 退出当前虚拟环境

deactivate
 4. 删除某个虚拟环境

rmvirtualenv my_env
5. 列出所有虚拟环境

lsvirtualenv
6. 进入到虚拟环境所在的目录

cdvirtualenv
修改 mkvirtualenv 的默认路径：

在 我的电脑->右键->属性->高级系统设置->环境变量->系统变量 中添加一个参数 WORKON_HOME ，将这个
参数的值设置为你需要的路径。

创建虚拟环境的时候指定 Python 版本：
在使用 mkvirtualenv 的时候，可以指定 --python 的参数来指定具体的 python 路径：

mkvirtualenv --python==C:\Python36\python.exe hy_env