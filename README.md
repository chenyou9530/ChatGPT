# ChatGPT
我們利用了ChatGPT建立起一套微信登入系統，目前功能可以操作的僅有登入按鈕，在註冊按鈕中我們建立了一個index.js的檔案，目的是將註冊成功的帳號寫入檔案裡面。

<img width="1284" height="1013" alt="image" src="https://github.com/user-attachments/assets/98dfcb81-f4b3-4ce6-b955-64fbcd7bfe51" />

接著跟GPT說請他修改CSS的樣式: <img width="773" height="466" alt="image" src="https://github.com/user-attachments/assets/00f22211-7a36-4e48-b21c-917f57c58099" />

<img width="1248" height="860" alt="image" src="https://github.com/user-attachments/assets/ce8e7d7d-d6e5-4a5c-89b0-cb7c3eea044b" />




之後請他修改一些程式碼可以作用在自動登入、記住帳號，以及登入跳轉畫面
#登入
<img width="783" height="880" alt="image" src="https://github.com/user-attachments/assets/25391400-546f-406d-898b-c93f05b108ee" />
# 記住帳號
當有登入過一次之後就會將帳號記住
<img width="1278" height="880" alt="image" src="https://github.com/user-attachments/assets/cf5bd688-9c3a-42bd-8116-6dfdb383e8be" />
# 自動登入
當帳號有成功登入之後 就會將帳號記住再次登入之後會直接登入
<img width="1271" height="735" alt="image" src="https://github.com/user-attachments/assets/c65bba9c-b439-4c10-a090-ac43a61821a3" />
# 登入跳轉畫面
登入之後就會跳轉到以下這個畫面
<img width="1291" height="875" alt="image" src="https://github.com/user-attachments/assets/ad6b01b1-3f90-439f-b89f-a176f5aa6d4f" />

# 註冊
但我們測試後雖然可以成功跳出註冊成功的畫面且重複按一次後會再跳出用戶已註冊，但是無法將帳號寫入index.js裡面，而註冊成功的帳號會被暫時用本地儲存 (wx.setStorageSync) 來模擬註冊後的帳號保存。

# 擴充功能
1.希望在註冊的方面可以利用SQL作為帳號資料的存儲，並將SQL掛載到js檔案裏面做新增讀取的功能，以及在註冊介面新增一個電話號碼以防止帳號被過度註冊而導致SQL儲存空間太大，並藉由電話號碼將帳號設定成專一性。

2.在個人資料中可以有比較完善的功能，例如登出按鈕，在登入錯帳號的時候可以用來重新登入。

# 缺點
1.自動登入:
經過我們在測試過後，無論是什麼帳號只要登入過後就會直接登入。
