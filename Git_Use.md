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
    - (失败) git pull origin master -- allow-unrelated-histories
    ```

  - ```
    push到远程仓库
    - git push origin master
    ```

    

#### 二、常用命令及其用法

##### 1、本地仓库操作 (**`时空穿梭`**)

- 查看仓库当前状态

  - git status
    
  - 没有内容发生变化

  - ![01](https://github.com/Minyonlew/TheUseOfGit/blob/master/01.PNG)

  - 有内容发生变化

  - ![02](https://github.com/Minyonlew/TheUseOfGit/blob/master/02.PNG)

- 查看修改内容

  - ```
    git diff
    ```

  - ![03](https://github.com/Minyonlew/TheUseOfGit/blob/master/03.PNG)

- 显示从最近到最远的提交日志

  - ```
    git log
    git log --pretty=oneline    (只显示提交时的备注 -m"xxx")
    ```

    ![04](https://github.com/Minyonlew/TheUseOfGit/blob/master/04.PNG)

- **版本回退**

  - ```
    git reset --hard 具体版本号	   (返回到具体版本)
    git reset --hard HEAD^		  (返回到上一个版本)
    git reset --hard HEAD^^		  (返回到上上一个版本)
    git reset --hard HEAD~100	  (返回到上100个版本)
    ```

  - 例子

    - ```
      git reset --hard xxxxxx	   (返回到具体版本)
      
      ```

    - 这里的版本号 可以通过命令 git log --pretty=oneline 查看

  - 如果又想回退到最新的，但是不知道版本号

    - ```
      git relog    (来得到之前的版本号)
      ```

      

    















