# cnad-hw2
Cloud Native Application Development HW2


⸻

📂 Repo 建立與操作說明

✅ Repo 創建與初始化
	•	建立公開 Repo：cnad-hw2
	•	修改 README.md 以說明作業內容與操作流程
	•	初始化 commit，並加入 .gitignore 及說明文件

✅ Branch 管理
	•	建立三個分支：
	•	main：主分支
	•	hw1-p：正確版本程式碼分支
	•	hw1-f：故意讓 GitHub Action 失敗的錯誤分支

✅ 程式碼內容
	•	hello.py：正確的 Hello World 程式
	•	broken_hello.py：語法錯誤的 Hello 程式（缺冒號），用來觸發失敗的 GitHub Action

✅ Issue 與 Template
	•	在 .github/ISSUE_TEMPLATE/ 中新增 hw-template.md
	•	建立一個以模板提交的 open 狀態 Issue

✅ Pull Request 操作
	•	hw1-p → main 建立成功 PR 並合併
	•	hw1-f → main 建立成功 PR 並合併
	•	每個 PR 都針對程式碼區塊進行留言互動

✅ GitHub Actions 工作流程
	•	建立 .github/workflows/python-check.yml 自動執行 Python Lint 檢查（使用 flake8）
	•	Action 步驟包含：
	•	安裝 flake8（額外步驟 1）
	•	執行 flake8 lint 檢查（額外步驟 2）
	•	成功紀錄：hw1-p PR 有通過 Action ✅
	•	失敗紀錄：hw1-f PR 因語法錯誤而失敗 ❌
