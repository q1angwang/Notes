# 连接github

1. git环境

2. 生成秘钥key
    `$ ssh-keygen -t rsa `
    连续三个回车，key就生成，默认存放路径：`/Users/wangqiang/.ssh`

3. 打开自己的Github主页，在settings里面设置`SSH and GPG keys`

4. 打开生成的`id_ras.pub`文件，将公钥公布给github，注意文件中的所有文本都要po上去。

5. 测试连接 
    `$ ssh -T git@github.com`
    第一次测试时会弹出警告，填yes后回车

6. 设置username和email
    $ git config --global user.name "wq"
    $ git config --global user.email "qiangwanghhh@gmail.com"
    在把本项目上传到github之前设置username和email，每次commit都会记录下username和email。





## 更新仓库

1. 选择一个仓库的`clone with ssh`，eg：
    $ git clone git@github.com:q1angwang/Notes.git


2. 操作本地仓库：
    $ git add .
    $ git commit -m'first commit'


3. 把本地仓库推送到远程仓库 ：
    $ git push origin master

