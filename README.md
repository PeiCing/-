# Anatomy-Bone-Game

# 109 年教育部教學實踐計畫 = 【探討多媒體影像協作搭配數位遊戲教學之策略對於大專運動員在課堂學習行為表現之影響】

# (一) 登入註冊系統

![image](https://github.com/PeiCing/Anatomy-Bone-Game/blob/main/img/%E7%99%BB%E5%85%A5%E8%A8%BB%E5%86%8A%E7%B3%BB%E7%B5%B1.PNG)

# connect.cs: 資料庫連線、登入、讀取使用者資料
  
  void getvalue(): 讀取使用者資料(含遊戲帳號密碼、中文遊玩紀錄、英文遊玩紀錄)
  
  void checkPW(): 檢查密碼

  void checkIDPW(): 檢查帳號是否註冊

  void Insert(): 登入
  
  void ConnectServer(): 資料庫連線

# SignIN.cs: 資料庫連線、使用者註冊

  void setvalue(): 設定玩家初始資料(含遊戲帳號密碼、中文遊玩紀錄、英文遊玩紀錄)
  
  void signin(): 使用者資料庫註冊
  
  void checkIDPW(): 檢查帳號
  
  void Insert(): 檢查欄位是否為空

  void ConnectServer(): 資料庫連線

# PlayGameBtn.cs: 點擊bottom換場景

# (二)、選擇語言頁面
![image](https://github.com/PeiCing/Anatomy-Bone-Game/blob/main/img/選擇語言.png)

# ADDLanguage.cs: 使用者遊玩紀錄(語言)

# (三)、遊玩介面
![image](https://github.com/PeiCing/Anatomy-Bone-Game/blob/main/img/遊玩介面.png)

# menuCN.cs: 一二三關卡的menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

# ClickSwith.cs: 遊玩選擇限制(模式、部位)
DoClickSwith(): 讓按鈕不能按

# ADDType.cs: 使用者遊玩紀錄(骨頭關卡或是肌肉關卡)

# ADDLevel.cs: 使用者遊玩關卡紀錄(第一關的手部、腿部、核心部位或第二關、第三關)

# ADDDirection.cs: 使用者遊玩方向紀錄(身體的正面或背面)

# ADDWay.cs: 使用者遊玩模式紀錄(拼圖、掃描、敲擊)

  Insert(string name): 放進資料庫
  
  Build(): 拼圖
  
  Scan(): 掃描
  
  Whack(): 敲擊
  
  ConnectServer(): 資料庫連線

MenuArmCh: 手臂的中文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

MenuLegCh: 腳部的中文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

MenuCoreCh: 核心的中文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

L2MenuCH: 第二關(全身無動作)的中文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

L3MenuCH: 第三關(全身有動作)的中文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式 
add(): 顯示按鈕旁邊的”完成”


MenuArmEg: 手臂的英文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

MenuLegEg: 腿部的英文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

MenuCoreEg: 核心的英文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

L2MenuENG: 第二關(全身無動作)的英文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

L3MenuENG: 第三關(全身有動作)的英文menu裡，控制顯示按鈕旁邊的”完成”。用於限制遊玩模式
add(): 顯示按鈕旁邊的”完成”

# 設計限制: 

須完成第一關才能往下第二關、第三關，且登出後要從第一關開始玩，不得越過關卡。

# 設計目的: 

讓學生重複練習，直到通關。使教授可藉由系統得知學生每次遊玩時的分數，看出進步成效。

# (四)、骨骼拼圖

![image](https://github.com/PeiCing/Anatomy-Bone-Game/blob/main/img/腳步拼圖.PNG)

# 玩法: 

利用滑鼠將骨頭拖移放置到左方人體上，平均分數超過80分為勝利，否則失敗。

# 說明: 

(1)	正確位置附近有範圍設定，若在範圍內放置則偵測為正確，否則彈回原位置。

(2)	最後列出每個骨頭放置正確所花費的時間，使教授與學生可以清楚得知較不熟悉的骨頭位置並加以複習。

# (五)、骨骼透視

![image](https://github.com/PeiCing/Anatomy-Bone-Game/blob/main/img/核心透視.png)

# 玩法: 

利用滑鼠點選透視鏡紅心開始遊戲，依據題目點選正確位置，平均分數超過80分為勝利，否則失敗。

# 說明: 

(1)	正確位置附近有範圍設定，若在範圍內點選則偵測為正確，否則彈回原位置。

(2)	最後列出每個骨頭點擊正確所花費的時間，使教授與學生可以清楚得知較不熟悉的骨頭位置並加以複習。

# (六)、骨骼敲擊

![image](https://github.com/PeiCing/Anatomy-Bone-Game/blob/main/img/全身敲擊.png)

# 玩法: 

利用滑鼠點選透視鏡紅心開始遊戲，依據題目點選正確位置，平均分數超過80分為勝利，否則失敗。

# 說明: 

(1)	正確位置附近有範圍設定，若在範圍內點選則偵測為正確，否則彈回原位置。

(2)	最後列出每個骨頭點擊正確所花費的時間，使教授與學生可以清楚得知較不熟悉的骨頭位置並加以複習。
