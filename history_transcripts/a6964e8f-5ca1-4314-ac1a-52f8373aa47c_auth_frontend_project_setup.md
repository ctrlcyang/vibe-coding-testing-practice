# Auth Frontend Project Setup

**Conversation ID**: `a6964e8f-5ca1-4314-ac1a-52f8373aa47c`


---


*(Executed tools: list_dir)*


### 🤖 Assistant

這個錯誤是因為 PowerShell 的執行原則（Execution Policy）限制了腳本執行，導致無法執行 `npm.ps1`。

### 解決方法 1：修改當前使用者的執行原則（推薦）

在 PowerShell 中執行以下指令：

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

---

### 解決方法 2：改用 `npm.cmd`

如果不方便修改執行原則，可以直接指定執行 `.cmd` 版本：

```powershell
npm.cmd install
```


### 👤 User

這樣算完成嗎


*(Executed tools: view_file)*


### 🤖 Assistant

是的，這樣就**已經安裝完成了**。

畫面上顯示 `added 348 packages`，代表專案所需的依賴套件已經成功下載並安裝。

至於下方的 `vulnerabilities`（安全漏洞）與 `funding`（贊助提示）是 `npm` 的正常警告與提醒，不影響專案的開發與執行。

### 下一步
您可以直接在終端機輸入以下指令來啟動開發伺服器：

```bash
npm run dev
```