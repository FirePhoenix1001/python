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
建立分支

    git  branch [名稱]

---
切換分支

    git switch [名稱]
---
分支內的儲存測試
1. 第一次
2. 第二次
3. 第三次

- 2026/04/10
---
## 存檔點

    git checkout [ID]
- 2026/04/17
---
## 刪除存檔點&合併存檔點
以下操作要非常小心  
刪除存檔點：把目標存檔點改成`drop`

    git rebase -i --root
---
## 合併存檔點
把目標存檔點改成`s`(squash的意思)，最推薦
- 2026/04/24
---
