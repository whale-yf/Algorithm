git使用



-git是一种用于版本控制的系统
    --创建一个github仓库
        ---github 创建
        ---远程创建 git remote add origin git@github.com:username/path
    --如果存在仓库可以通过clone创建一个副本
        ---clone本地仓库 git clone /path
        ---clone远程仓库 git clone username@host:username/path
-git工作流程
    --git工作结构：工作区 ==> 缓冲区(index) ==> HEAD
        ---工作区：所要提交的文件目录的地方
        ---缓冲区：临时保存改动
        ---HEAD：指向最后的提交结果
    --git add <filename> 将工作区改动临时保存
    --git commit -m 'content of change' 将临时保存的改动提交至HEAD
    
    --git push origin master/branch 提交HEAD至目标host

-git结构
    --master:在创建仓库是会同时创建一个master目录，可以理解为根目录
    --branch:相当于根目录下的子目录，同时可以合并至master
        ---git checkout -b <filename> 创建一个branch
        ---git checkout -d <filename> 删除一个branch
        ---git checkout master 切回至master checkout 切回命令
        ---如果不将branch 推送到远程仓库，别人就不会看见
        ---git merge<branch> 将branch合并到master
-git 常用运维
    --git log 查看日志
    --git tag 标签，暂时还未使用  ！！！！！
    
