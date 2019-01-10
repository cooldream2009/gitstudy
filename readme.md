本项目主要用来学习git的知识。

采用边学边记录的方式，说明文件也会随着知识内容的更新而更新。

将git的默认编辑器设置为sublime后，如果使用git commit命令，则会自动打开sublime，填入commit的说明，然后关闭sublime，则git commit执行完成。注意，如果一开始sublime是打开的状态，或者sublime没有关闭，都不会完成提交的动作。

设置github为远程仓库，比如https://github.com/cooldream2009/gitstudy，需要先在github上面新建一个空的gitstudy仓库，然后再使用git命令将本地仓库push到gitstudy上。如果再github上创建仓库的时候，初始化了仓库，则需要先将仓库pull到本地，然后修改，再进行push。

解决每次都输入用户名密码的问题。参考https://www.jianshu.com/p/81ae6e77ff47，命令行中输入
> git config --global credential.helper store

再想远程仓库push一下，输入用户名密码，这时候，用户名密码就会被记录下来保存，以后再push的时候就不用输入用户名密码验证了。

也可以直接在C:/Users/username目录（username为计算机用户名），新建一个文件.git-credentials，文件内容就一行文字，为https:{username}:{password}@github.com，username和password对应自己的github用户名密码。然后在命令行输入git config --global credential.helper store。