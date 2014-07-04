
LightPods
==========

## 开发流程
#### 添加pod源
    $ pod repo add LightSDK https://github.com/LightCircle/LightPods

#### 新建工程
使用xcode创建工程

进入工程，生成pod文件

    $ pod init

指定LightSDK依赖

    $ vi Podfile
    
    target "Your projects" do
      pod 'LightSDK', '~> 0.0.1'
    end

#### 安装pod依赖
    $ pod install

----

## pod相关操作
http://cocoapods.org/

#### 安装pod
    $ sudo gem install cocoapods

#### pod升级
    $ sudo gem update --system
    $ sudo gem update cocoapods

#### 确认po的版本
    $ pod --version

#### gem本身的升级
    $ sudo gem update --system

## pod问题对应
#### 执行pod命令出现警告
    warning: Insecure world writable dir /usr/local in PATH, mode 040777

要去除这个警告，需要更改/usr/local的权限，一句话：

    $ sudo chmod go-w /usr/local
