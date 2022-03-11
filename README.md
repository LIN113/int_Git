# int_Git
Git的初步使用
一、通过homebrew安装Git
    1、未安装homebrew，需安装homebrew
        /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    2、安装git
         brew install git

二、创建用户和邮箱
    1、创建全局用户名和邮箱（你的Github邮箱），终端内输入
        git config --global user.name "此处填写你本地的用户名"
        git config --global user.email "此处填写你Github的邮箱"
        查看git配置信息：git config --list
    2:创建ssh key
        ssh-keygen -t rsa -C "此处填写你Github的邮箱"
    3：cat命令查看key
        cat .ssh/id_rsa.pub

三：在GitHub中添加ssh key
    点击Settings-->点击New SSH key-->添加key

四：验证连接
        ssh -T git@github.com       


参考信息：
https://www.jianshu.com/p/7edb6b838a2e
https://blog.csdn.net/qq_44818523/article/details/108997078
