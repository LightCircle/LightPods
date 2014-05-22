
SmartPods
==========

## 开发流程
#### 添加pod源
    $ pod repo add SmartSDKIOS https://github.com/SmartCircle/SmartPods

#### 新建工程
1. 使用xcode创建工程
2. 进入工程，生成pod文件

    $ pod init

3. 指定SmartSDK依赖

    target "LikeIOS" do
      pod 'SmartSDK', '~> 0.0.1'
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
