# Correlation IDs

## 需求
在分散式系統架構(微服務架構)中，通過各種組件了解單個end to end客戶交易流程是很困難的。

以下是一些普遍會遇到的挑戰：
* 了解客戶請求進入應用程序的end to end行為變得有挑戰性
* 聚合：整合來自多個元件的日誌，並理解這些日誌是困難的。
* 對服務、事件流程和非同步請求的循環依賴不容易解譯。
* 對於請求故障排除時，日誌的診斷情境對於找到真因是很重要的。

## 解法

Correlation  ID 是一個唯一標識符，它被添加到第一個傳入請求中以標識上下文，並傳遞給事務流中涉及的所有組件。
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzg2OTU3ODYsLTQ1NTU1NzIsLTE4MDI4Nj
A2MzEsMTM3MzkyOTYyNV19
-->