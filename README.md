# 學習 Git 版本控制，持續更新
## 項目
- [建立版本管理庫](#建立版本管理庫)
- [記錄操作](#記錄操作)
- [提交返回](#提交返回)
- [分支](#分支)
## 建立版本管理庫
* 設定個人資訊(config)
    * 每次在Git commit都會記錄作者訊息(Name與Email)

        `git config --global user.name "<你的名字>"`

        `git config --global user.email "<你的Mail>"`
    * 查看個人設定

        `git config --global --list`
* 建立版本管理庫(init)

    `git init`
* 新增文件管理(add)
    * 新增文件

        `git add <檔名>`
    * 一次新增所有文件

        `git add .`
* 提交變更(commit)

    `git commit -m "<變更資訊>"`
* 修改變更(amend)

    `git commit --amend -m "<變更資訊>"`
## 記錄操作
* 查看記錄(log)

    `git log`
* 查看工作目錄下所有檔案情況，Project、modified、untracked、new file，最後參數s是用最簡潔方式印出結果

    `git status -s`
* 查看尚未add(unstaged)的修改部分

    `git diff`
* 查看已add(staged)，但未commit，在最後加入參數cached

    `git diff --cached`
* 查看unstaged & staged，在最後加入 HEAD

    `git diff HEAD`