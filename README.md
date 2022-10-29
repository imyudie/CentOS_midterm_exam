## CentOS_midterm_exam攻略

### 在開始之前請先變更主機名稱為你的"學號.cyut.edu.tw"

Step1: 開啟一個終端機視窗  
Step2: sudo nano /etc/hostname  
Step3: Update the host name  
Step4: Ctrl+O 存檔  
Step5: Ctrl+X 退出 nano  
Step6: 登出在重新登入  


### 1.變更操作界面成為繁體中，但用戶home目錄資料夾名稱不可變更(10%)
Step1: 到右上角Application > System Tools > Setting 並到Region & Language  
![image](https://user-images.githubusercontent.com/102812213/198816317-91a81214-7a74-4273-9e41-da089f525664.png)
  
Step2: 在Language上點一下，點選下方三個點，輸入chinese然後選"漢語(台灣)"  
![image](https://user-images.githubusercontent.com/102812213/198816517-cddc032f-892f-40ce-ab4f-15daaa07aa2f.png)
  
Step3: 重新啟動(點那個Restart就好)  
![image](https://user-images.githubusercontent.com/102812213/198816711-9a23bf18-5dad-4121-b4bd-4249768c8f3c.png)
  
Step4: 若是遇到他要求更換資料夾名稱，請拒絕更換。
  
### 2.請安裝中文Chewing輸入法，並設定為Ctrl + 空白鍵進行切換(10%)
Step1: 到設定中的地區與語言，點選輸入來源下的加號  
![image](https://user-images.githubusercontent.com/102812213/198817045-c464ec73-8e58-4b98-b34c-bd07c19ef51c.png)
  
Step2: 點選漢語(台灣) > 漢語(Chewing) > 加入(A)  
![image](https://user-images.githubusercontent.com/102812213/198817113-759c342c-2d11-448c-98ae-aa358c51309f.png)
  
Step3: 到設定 > 裝置 > 鍵盤 > 鍵盤快捷鍵 > 切換到下一個輸入來源 > (按Ctrl + 空白建) > 設定  
![image](https://user-images.githubusercontent.com/102812213/198817306-c0c3b74e-0a1e-450c-ba02-8a64f716a3f1.png)
  
### 3.調整畫面解析度為 1280 x 960 (5%)  
Step1: 設定 > 裝置 > 顯示器 > 解析度 > 1280x960 > 套用  
![image](https://user-images.githubusercontent.com/102812213/198817774-59a65242-e3e4-4960-a5ec-23916455d715.png)
  
### 4.請列出如何在終端機模式下，讓系統等候3分鐘後關機的指令 (10%)
```Linux
sudo shutdown -h +3
```
  
### 5.請列出如何在終端機模式下，讓系統等候5分鐘後重新啟動，並顯示"System will be reboot after 5 mins"的用戶通知，指令 (10%)
```Linux
sudo shutdown -r +5 System will be reboot after 5 mins
```
  
### 6.關閉GUI系統模式下，螢幕自動鎖定的功能 (5%)
Step1: 設定 > 電源 > 螢幕轉黑 > 永不  
![image](https://user-images.githubusercontent.com/102812213/198818995-33bb665b-6619-4c6b-b455-1ceaaed1c16e.png)

### 7.請在終端機模式下，利用指令顯示出目前系統時間，顯示格式為"西元年(4碼)/月(2碼)/日(2碼) 時(2碼):分(2碼):秒(2碼) (10%)
```Linux
date '+%Y/%m/%d %H:%M:%S'
```
  
### 8.請在終端模式下，利用cal 指令列出今天是今年的第幾天(1~365) (5%)
```Linux
cal -j
```
  
### 9.用nano 在終端機模式下，編輯一個檔名為"學號.txt"的檔案且內容如下存檔後並上傳。 (10%)
　檔案內容如下：  
　班級：  
　姓名：  
　學號：  
Step1: 開啟終端機並輸入  
```Linux
nano your_student_ID.txt
```
Step2: 照規定輸入格式，以下是範例  
![image](https://user-images.githubusercontent.com/102812213/198820524-f38d061b-b23f-42a8-946a-253b4e836f2e.png)
Step3: "Ctrl + O"寫入檔案，"Ctrl + X"離開nano  

### 10.請將"學號.txt"此檔案的權限變更設定如下 (10%)：
　OWNER：可讀、可寫、可執行 = 111(2) = 7  
　GROUP：可讀、可執行 = 101(2) = 5  
　OTHER：可寫、可執行 = 011(2) = 3  
Step1: cd至學號.txt目錄，輸入
```Linux
sudo chmod 753 your_student_ID.txt
```
  
### 11.請將"學號.txt"此檔案的擁有者變更為 root，群組設定為 users (10%)
```Linux
sudo chown root:users your_student_ID.txt
```
  
### 12.在終端機模式下，如何列出所有包含隱藏檔案在內，的檔案詳細資料 (5%)
```Linux
sudo ls -al
```

###每一題須繳交資料如下檔案名稱也必須一致：
1.上傳畫面截圖 Chinese.png  
2.上傳畫面截圖 Chewing.png  
3.上傳畫面截圖 Resolution.png  
4.上傳畫面截圖 Shutdown.png  
5.上傳畫面截圖 Reboot.png  
6.上傳畫面截圖 Blankscreen.png  
7.上傳畫面截圖 Date.png  
8.上傳畫面截圖 Calendar.png  
9.上傳畫面截圖 學號.txt  
10.上傳畫面截圖 Chmod.png  
11.上傳畫面截圖 Chown.png  
12.上傳畫面截圖 Ls.png  
