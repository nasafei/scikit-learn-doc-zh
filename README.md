# scikit-learn-doc-zh
scikit-learn 官方文档-中文版

## 安装 virtualenv 和 virtualenvwrapper 来管理环境

> 安装 python

`参考链接： http://www.tuicool.com/articles/aueyMn`
brew install python3

> 安装 pip

```
wget https://bootstrap.pypa.io/get-pip.py
python3 get-pip.py
```

> 安装 virtualenv 和 virtualenvwrapper

```
sudo pip3 install virtualenv
sudo pip3 install virtualenvwrapper

-- 查找 virtualenvwrapper 安装路径 (Mac在 /Library/Frameworks/Python.framework/Versions/3.5/bin/virtualenvwrapper.sh)
find / -name virtualenvwrapper.sh

mkdir ~/.virtualenvs
vim ~/.bash_profile (`source ~/.bash_profile`)

export WORKON_HOME=~/.virtualenvs
export VIRTUALENVWRAPPER_PYTHON=/Library/Frameworks/Python.framework/Versions/3.5/bin/python3.5
source /Library/Frameworks/Python.framework/Versions/3.5/bin/virtualenvwrapper.sh
```

> 创建虚拟环境

```
mkvirtualenv -p /Library/Frameworks/Python.framework/Versions/2.7/bin/python python2
mkvirtualenv -p /Library/Frameworks/Python.framework/Versions/3.5/bin/python3.5 python3
```

> 虚拟环境的其他操作

```
启动: source ~/.virtualenvs/python3/bin/activate
lsvirtualenv: 列出虚拟环境列表
mkvirtualenv: 新建虚拟环境
workon [虚拟环境名称]: 切换虚拟环境
rmvirtualenv: 删除虚拟环境
deactivate: 离开虚拟环境 ( source deactivate )
```

## 不想安装 virtualenvwrapper 也可以

```
cd /home/
mkdir ~/pyEnv
virtualenv -p /Library/Frameworks/Python.framework/Versions/2.7/bin/python env_py2
virtualenv -p /Library/Frameworks/Python.framework/Versions/3.5/bin/python3.5 env_py3

-- 启动
source env_py3/bin/activate 
-- 关闭
deactivate 
```

## pip 安装 相关插件

```
-- WARNING: LaTeX command 'latex' cannot be run (needed for math display), check the imgmath_latex setting
-- 安装latex: http://www.tug.org/mactex/morepackages.html

sudo pip3 install image
sudo pip3 install matplotlib
sudo pip3 install docutils==0.12
sudo pip3 install nose
sudo pip3 install numpy
sudo pip3 install scipy
sudo pip3 install sphinx==1.4.5
sudo pip3 install scikit-learn
```
