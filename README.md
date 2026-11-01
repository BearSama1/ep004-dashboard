# EP004 艦隊狀態（唯讀）

呢個係自動發佈嘅唯讀狀態頁，顯示 EP004 研究線路係咪運行緊、用緊咩模型、研究緊咩，同埋 token 用量。

- 網頁：https://bearsama1.github.io/ep004-dashboard/
- 數據：`data` 分支嘅 `status.json`，由發佈程式每約 60 秒覆寫一次（單一 commit，force-push），推送前會做敏感資料檢查。
- 網頁每 90 秒經 GitHub contents API 讀取數據（未登入限額每小時 60 次）；失敗時改讀 raw.githubusercontent.com（CDN 可能延遲最多約 5 分鐘）。
- 冇按鈕、冇表單，唔會向任何研究程式發指令。

This is an auto-published, read-only status page. Data lives on the `data` branch and is overwritten roughly every 60 seconds.
