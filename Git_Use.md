#### 一、简略创建仓库并提交到远程仓库

- 初始化仓库

  - ```git
    git init
    ```

- 添加文件

  - ```
    git add -A(全部文件)
    git add -xxx(提交指定文件）
    ```

- 提交文件

  - ```
    git commit -m "提交时附带的注释"
    ```

- 查看当前仓库状态

  - ```
    git status
    ```

- 关联到远程仓库

  - ```
    git remote add origin git@github.com:Minyonlew/TheUseOfGit.git
    ```

- 将文件推送到远程仓库

  - ```
    （第一次推送）先要pull 下来
    - (正常) git pull origin master
    - (失败) git pull origin master -- allow-nurelated-histories
    ```

  - ```
    push到远程仓库
    - git push origin master
    ```

    

#### 二、常用命令及其用法

##### 1、本地仓库操作 (**`时空穿梭`**)

- 查看仓库当前状态

  - ```
    git status
    ```

  - 没有内容发生变化

    









