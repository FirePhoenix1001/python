# git 介紹
git就像一個可以存檔工具

    git init
---

把檔案納入追蹤和儲存

    git add [path]
---

幫存檔命名

    git commit -m "內容"
---

- `git add` 和 `git commit -m` 一起搭配，先儲存後命名

1. 第一次
2. 第二次
3. 第三次

---
回去存檔點的指令(不建議太危險)

    git reset [存檔點ID]

- 2026/03/27
---
## 分支
查看目前的分支

    git branch
---
建立新分支

    git branch [名稱]
---
切換分支

    git switch [名稱]
---
分支內的儲存測試
1. 第一次
2. 第二次
3. 第三次
---
當我發現我應該寫在另一個分支時

    git stash
    git switch [名稱]
    git stash pop
---
刪除分支(本地)

    git branch -D [名稱]

刪除分支(遠端)(不建議太危險)

    git push origin --delete [名稱]

- 2026/04/10
---
## 存檔點
查看存檔點

    git checkout [存檔點ID]
---
## 刪除存檔點&合併存檔點
以下操作要非常小心  
刪除存檔點：把目標存檔點改成`drop`

    git rebase -i [存檔點ID]
---
合併存檔點兩種方式  
指標合併(不靈活)

    git reset --soft HEAD~[數字]
    git commit -m "合併後的訊息"
---
把目標存檔點改成`squash`，最推薦

    git rebase -i [存檔點ID]
---
## 線上操作
取得線上的「存檔點」，前提是本地沒有多出先上沒有的存檔點

    git pull origin [分支名稱]
---
強制同步：兩步驟  
第一步：取得線上的「存檔點」

    git fetch origin [分支名稱]

第二步：把本地的「存檔點」改成線上的「存檔點」

    git reset --hard origin/[分支名稱]
---
強制推送

    git push origin [分支名稱] --force

- 2026/04/17
---