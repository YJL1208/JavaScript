# NPM

自己积累的一些npm用法

## 目录

* [npm查看全局安装](#npm查看全局安装)
* [配置npm默认的环境变量](#配置npm默认的环境变量)
* [安装淘宝镜像cnpm](#安装淘宝镜像cnpm)


### npm查看全局安装

    npm list --depth --global
<br>
<br>

### 配置npm默认的环境变量

1.配置npm的全局模块的存放路径以及cache的路径

    npm config set prefix "D:\Program Files\nodejs\node_global"

	npm config set cache "D:\Program Files\nodejs\node_cache"   


2.在系统环境中添加系统变量NODE_PATH，输入路径，此后所安装的模块都会安装到改路径下

    D:\Program Files\nodejs\node_global\node_modules

3.在配置系统环境path

	D:\Program Files\nodejs\node_global


4.在命令行输入以下命令试着安装express，安装完毕后可以看到.\node_global\node_modules\express 已经有内容

	npm install express -g

<br>
<br>

### 安装淘宝镜像cnpm

1.安装cnpm

	npm install -g cnpm --registry=https://registry.npm.taobao.org

2.配置环境路径

	cnpm会被安装到D:\Program Files\nodejs\node_global下


**注意**

	如果系统变量path并未包含该路径。在系统变量path下添加该路径即可正常使用cnpm。

3.cnpm -v 验证

