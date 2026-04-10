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
回去存檔點的指令

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

    git branch -d [名稱]

刪除分支(遠端)

    git push origin --delete [名稱]

- 2026/04/10
---
