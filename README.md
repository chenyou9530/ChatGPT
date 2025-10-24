# ChatGPT
我們利用了ChatGPT建立起一套微信登入系統，目前功能可以操作的僅有登入按鈕，在註冊按鈕中我們建立了一個index.js的檔案，目的是將註冊成功的帳號寫入當按裡面。
<img width="423" height="864" alt="image" src="https://github.com/user-attachments/assets/a9ffd522-4053-43ba-9f63-09ce5b4ad44c" />
<img width="392" height="783" alt="image" src="https://github.com/user-attachments/assets/50018f82-ef3f-4dc5-b5b1-e520453572e7" />

<img width="426" height="791" alt="image" src="https://github.com/user-attachments/assets/e03473fb-c954-4d77-89d3-e0fdd93659a6" />
<img width="369" height="197" alt="image" src="https://github.com/user-attachments/assets/d3e6cbe5-a35b-405f-8f22-9ff47d479460" />
但我們測試後雖然可以成功跳出註冊成功的畫面且重複按一次後會再跳出用戶已註冊，但是無法將帳號寫入index.js裡面，而註冊成功的帳號會被暫時用本地儲存 (wx.setStorageSync) 來模擬註冊後的帳號保存。
<img width="780" height="453" alt="image" src="https://github.com/user-attachments/assets/5b3814be-9172-43d3-a5ae-9309874d9d58" />
