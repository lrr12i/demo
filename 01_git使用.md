# Git
## 配置
    name
        git config --global user.name "lrr"
    email
        git config --global user.email "lrr12i@163.com"

## 使用git
    git status 
        查看仓库状态
            已跟踪
                暂存：文件修改已保存，但是未提交到git仓库
                未修改：磁盘中的文件和git仓库中文件相同，没有修改
                已修改：磁盘中文件已被修改，和git仓库中文件不同
                已修改 -> 暂存 -> 仓库
            未跟踪
                刚添加的文件

                git add <filename>
                git add *
                    未跟踪-->暂存
                    将文件切换到暂存状态

                git commit -m "第一次提交1.txt"
                    暂存-->未修改
                    将暂存的文件存储到仓库中

                    未修改-->修改
                    修改代码后，文件变修改状态

                git commit -a -m ""
                    提交所有已修改文件(未跟踪文件不会提交)
                
                git init
                    初始化仓库

    重置文件：
        git restore <filename>
            恢复文件
        git restore --staged <filename>
            取消暂存状态

    删除文件：
        git rm <filename>
            删除文件
        git rm <filename> -f
            强制删除文件

        移动文件：
            git mv from to
            移动文件 重命名文件
    
## 远程库
    操作命令
        git remote add <name> <url>
            添加远程库
        git branch -M main
            修改主分支的名字
        git push -u <name> main
            上传推送
        git remote remove <name>
            删除远程库
        git remote
            查看当前关联远程库
    
