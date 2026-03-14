# Team 5 Project

## Team Members
* **Gabby**

---

## Git Development Workflow

### 1. Create a New Branch
* **Command:**
```bash
# 切換到主分支
git checkout main
# 從遠端拉取最新程式碼
git pull origin main
# 建立並切換到新分支(feature/task-description建議可以直接從這個名稱看出改了啥)
git checkout -b feature/task-description
```

### 2. Implementation & Commit
```bash
# 查看變更狀態
git status
# 將變更加入暫存區
git add .
# 提交變更 (提供具體的commit message)
git commit -m "feat: implement unclosed block checking for flash analysis"
```

### 3. Push & Pull Request
```bash
# 推送分支
git push origin feature/task-description
```

### 4. Merge & Cleanup
```bash
# 切換回 main 並更新
git checkout main
git pull origin main
# 刪除已合併的本地分支(不一定要)
git branch -d feature/task-description
```
