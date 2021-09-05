##### 1.前後端差異

前端主要負責瀏覽器上畫面的呈現(顏色.區塊）；後端則是依照請求將特定處理資料與資料庫溝通等等。

##### 2.在google首頁搜尋JavaScript並按下Enter到看到搜尋結果所發生的事情

1. 瀏覽器送出關鍵字給google的server
2. google server 去資料庫搜尋關鍵字並取得結果
3. google server 將結果回傳
4. 瀏覽器顯示搜尋結果

##### 3.在(2)加入DNS server, cache概念

1. 瀏覽器在送出關鍵字JavaScript到google.com
2. 瀏覽器檢查DNS cache有沒有儲存google.com的IP位置
3. 有的話就發送request到IP位置
4. 沒有的話，呼叫C語言提供的function（c語言是因為chrome多是用c語言撰寫的）
5. C語言呼叫作業系統
6. 作業系統檢查DNS cache有沒有儲存google.com
7. 有的話回傳位置
8. 沒有的話去DNS server（8.8.8.8)查google.com的IP位置
9. DNS server回傳給IP位置（172.217.160.78)
10. 瀏覽器發送request到該IP位置（172.217.160.78)
11. google server收到資料 去資料庫搜尋關鍵字並取得結果
2. google server 將結果回傳
3. 瀏覽器顯示搜尋結果