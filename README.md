# Team 5 Project

## Team Members
* **Gabby**

---

## Git Standard Operating Procedure (SOP)

### 1. Create a New Branch
```bash
# 切換到主分支
git checkout main
# 從遠端拉取最新程式碼
git pull origin main
# 建立並切換到新分支
# 建議格式: <type>/<description> (例如: fix/a_bug)
git checkout -b <branch_name>
```

### 2. Implementation & Commit
```bash
# 更新本地的 main 資訊
git fetch origin main

# Sync with Main
git rebase origin/main

# 如果發生衝突 (Conflict)：
# 1. 手動修改檔案解決衝突
# 2. git add <file_name>
# 3. git rebase --continue
# (若想放棄 rebase 回到原狀，執行 git rebase --abort)
```

### 3. Implementation & Commit
```bash
# 查看變更狀態
git status
# 將變更加入暫存區
git add .
# 提交變更 (提供具體的commit message)
git commit -m "feat: implement unclosed block checking for flash analysis"
```

### 4. Push & Pull Request
```bash
# 推送分支
git push origin <branch_name>
```

### 5. Merge & Cleanup
```bash
# 切換回 main 並更新
git checkout main
git pull origin main
# 刪除已合併的本地分支
git branch -d <branch_name>
# 刪除遠端分支 (徹底從 GitHub 移除)
git push origin --delete <branch_name>
```
