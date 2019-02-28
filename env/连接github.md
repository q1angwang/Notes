# 连接github


1. git环境


2. $ ssh-keygen -t rsa 
生成用于连接Github的秘钥key，连续三个回车，key就完成生成了。
认存放路径为：`/Users/wangqiang/.ssh`


3. 打开自己的Github主页，在settings里面设置`SSH and GPG keys`


4. 打开生成的`id_ras.pub`文件，将公钥公布给github，注意文件中的所有文本都要po上去。


5. 测试连接 
`$ ssh -T git@github.com`

在第一次测试时会弹出警告，需要填写yes，然后回车




6. 设置username和email

在把本项目上传到github之前还需要分别输入设置username和email，因为github每次commit都会记录他们。所以分别输入如下命令：

$ git config --global user.name "wq"
$ git config --global user.email "qiangwanghhh@gmail.com"







## 附，更新仓库的过程：

1. 选择一个仓库的clone with ssh

    $ git clone git@github.com:q1angwang/Notes.git


操作本地仓库：
    $ git add .
    $ git commit -m'first commit'


2. 把本地仓库推送到远程仓库 ：

    $ git push origin master

