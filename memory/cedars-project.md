# CEDARS Project Shared Memory
> 由本地Cursor Agent 與 Grok Bot 共用記憶庫
> 標籤範例：【tag:cedars-company-data】

## 記憶列表

【tag:memory-rules】共用記憶庫操作規則（2026-10-13 由使用者制定）
- 每次開啟新任務，第一步：pull 倉庫 agent-shared-memory 最新內容，讀取 memory/cedars-project.md 全部歷史記憶。
- 只記錄關鍵業務資訊：專案決策、研究結論、檔案路徑、規則、待辦、約束條件；不存閒聊。
- 每條記憶開頭加標籤，例如【tag:cedars-company-data】。
- 資訊有更新時直接修改舊記錄，不重複堆疊；未經明確要求不得刪除舊記憶。
- 修改後必須 commit 並 push 回倉庫，commit message 簡潔，例如：add memory：CEDARS專案腳本資訊

【tag:cedars-company-data】CEDARS專案：Origin倉庫 cedars-company-data，執行 scripts/build_documents.py 從CSV重建docx/xlsx。
