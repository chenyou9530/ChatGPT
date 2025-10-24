# ChatGPT
我們利用了ChatGPT建立起一套微信登入系統，目前功能可以操作的僅有登入按鈕，在註冊按鈕中我們建立了一個index.js的檔案，目的是將註冊成功的帳號寫入檔案裡面。

<img width="423" height="864" alt="image" src="https://github.com/user-attachments/assets/a9ffd522-4053-43ba-9f63-09ce5b4ad44c" />
<img width="392" height="783" alt="image" src="https://github.com/user-attachments/assets/50018f82-ef3f-4dc5-b5b1-e520453572e7" />

<img width="426" height="791" alt="image" src="https://github.com/user-attachments/assets/e03473fb-c954-4d77-89d3-e0fdd93659a6" />


但我們測試後雖然可以成功跳出註冊成功的畫面且重複按一次後會再跳出用戶已註冊，但是無法將帳號寫入index.js裡面，而註冊成功的帳號會被暫時用本地儲存 (wx.setStorageSync) 來模擬註冊後的帳號保存。
<img width="369" height="197" alt="image" src="https://github.com/user-attachments/assets/d3e6cbe5-a35b-405f-8f22-9ff47d479460" />
<img width="780" height="453" alt="image" src="https://github.com/user-attachments/assets/5b3814be-9172-43d3-a5ae-9309874d9d58" />

此外我們在登入判斷是否成功後會跳轉到新增個人暱稱的畫面中
<img width="424" height="979" alt="image" src="https://github.com/user-attachments/assets/c750d176-1a0d-40a7-8f22-bed3b5e02abf" />

#擴充功能
1.希望在註冊的方面可以利用SQL作為帳號資料的存儲，並將SQL掛載到js檔案裏面做新增讀取的功能，以及在註冊介面新增一個電話號碼以防止帳號被過度註冊而導致SQL儲存空間太大，並藉由電話號碼將帳號設定成專一性。

2.在個人資料中可以有比較完善的功能，例如登出按鈕，在登入錯帳號的時候可以用來重新登入。
