# 潘冠伶(Gwen Pan)

+ Education:南臺科技大學 / 資訊管理系
+ Location: Tainan City
+  E-mail: gwenlyn.pan@gmail.com
+ Mobile: 0908-780-157

***
### 專業技能

+ 使用並基礎了解後端運作 PHP,資料庫及 MySQL 語法。
+ MySQL分析繪製E-R Model、規劃Table Schema，以及利用SQL關聯式資料庫進行資料查詢及處理。
+ Visual studio 利用C#語言撰寫Windows Forms App(.Net Framework)。
+ 使用爬蟲更新資料庫內容。


---
### 作品集
# [股價查詢系統](https://github.com/gwlpoxz/Stock_Price_System)

![圖片名稱](https://github.com/gwlpoxz/Resume/blob/main/index.png)
__使用爬蟲抓取台灣公開股價頁資料存入資料庫後， 撰寫php顯示在網頁中__

```text
/stock_analysis_system (專案根目錄)
│
├── config/                  # 系統配置與環境設定
│   └── db.php                # 資料庫連線與 Session 初始化
│
├── public/                  # Web 進入點與前端視圖 (UI)
│   ├── index.php             # 系統主控儀表板
│   ├── login.php             # 使用者登入頁面
│   ├── register.php          # 新使用者註冊頁面
│   ├── forgot.php            # 密碼重設引導頁
│   └── logout.php            # 登出與 Session 銷毀
│
├── api/                     # 處理特定請求的後端服務
│   └── export_handler.php    # 負責 Excel 報表生成與下載流
│
├── core_scripts/            # 數據處理核心 (ETL)
│   ├── twse_sync.py          # Python 爬蟲與數據同步引擎
│   └── run_stock_crawler.bat # Windows 環境啟動批次檔
│
└── logs/                    #存放執行日誌
    └── crawler_error.log     # 記錄 Python 執行失敗的 Traceback
```
<br>
<br>

# [web手寫數字辨識](https://github.com/gwlpoxz/mnist-web-app)

<img src="https://github.com/gwlpoxz/Resume/blob/main/mnist.png" width="400" alt="Sound Travel">
<br>
__結合deep Learning、computer vision、web開發的專案，<br>
透過訓練卷積神經網路CNN，並使用 **Flask** 搭建後端 API來辨識手寫數字，<br>
利用簡易互動式web介面，使用者可以即時塗鴉書寫 0-9 的數字，<br>
系統就會透過後端的 PyTorch模型進行即時分類就能辨識結果。__
<br>
#### 功能特色
+ 手寫畫布：支援滑鼠與觸控操作，提供直覺的手寫體驗。
+ 即時辨識：後端載入預訓練的 CNN 模型，辨識準確率高。
+ 響應式設計：介面簡潔，適配多種螢幕尺寸。

#### 核心技術
+ 深度學習框架: PyTorchs,Torchvision
+ 後端框架: Flask (Python)
+ 前端技術: HTML5 Canvas, CSS3, JavaScript
+ 圖像處理: Pillow (PIL), Torchvision__, NumPy

```text
mnist-web-app/
├── app.py                # Flask 後端主程式
├── train.py              # CNN 模型訓練腳本
├── mnist_cnn.pth         # 訓練完成的模型權重檔
├── templates/            # 存放 HTML 檔案
│   └── index.html        # 前端網頁主體
└── static/               # 存放 CSS 與 JS 靜態檔案
    ├── style.css         # 網頁樣式 (對應staticstyle.css)
    └── main.js           # 畫布互動與 API 呼叫邏輯
```
<br>
<br>

# [SoundTravel_Andoid APP]()



<img src="https://github.com/gwlpoxz/Resume/raw/main/soundtravel.jpg" width="400" alt="Sound Travel">

__利用爬蟲爬取公開網站JSON應用<br>
點擊台灣地圖位置隨即播放當地生態園區聲音<br>__

#### 程式碼重點
+ (1)依續建立地點清單、GPS位置、政府公開平台資訊網址<br>
    設定4個空清單存放讀取網站資料<br>
+ (2)每當地點被點選時:<br>
    取得變數清單內容<br>
    放大地圖至17<br>
    網路資料GET<br>
+ (3)每當網路取得文字時<br>
    確定回應代碼OK=200<br>
    存入變數解碼後的Json<br>
    複製內容存入allData<br>
    隨機選擇清單項目存入selectdata<br>
    讀取關鍵字資料存入selectmp3<br>
<br>
<br>
# [AI大圖搜索與精準點擊專案](https://github.com/gwlpoxz/WEEK01)
<br>
實作了一套基於 強化學習 (Reinforcement Learning, RL) 的高階觀察者系統。<br>
AI 代理人必須在 10000×10000的全域空間中，<br>
透過 800×800的有限局部視窗搜尋動態目標。<br>
<br>
<br>

#### 核心技術
   + 強化學習框架: Stable Baselines3 (SB3), Gymnasium
   + 深度學習底層: PyTorch
   + 強化學習演算法: PPO (Proximal Policy Optimization)
   + 模擬器與視覺化: Pygame
   + 數據處理與分析: NumPy, Pandas
   + 訓練監控技術: TensorBoard (TensorFlow)
   + 核心架構技術:
       + 模仿學習 (Imitation Learning): 行為克隆 (Behavioral Cloning)
       + 持續學習 (Continual Learning): 權重增量繼承機制
       + 座標映射技術: 全域與局部座標非線性變換 (Global-to-Local Mapping)
       + 獎勵塑造 (Reward Shaping): 距離感應與效率導向之獎勵函數設計
       
#### 專案架構
```text
   2 ├── rl_human_recorder.py      # [主程式] 專家數據錄製與互動介面
   3 ├── rl_pretraining.py         # [主程式] 模仿學習預訓練系統 (BC)
   4 ├── rl_machine_training.py    # [主程式] 機器增量強化訓練系統 (PPO)
   5 ├── rl_ai_demo.py             # [主程式] AI 成果效能驗證展示介面
   6 ├── hunter_latest.zip         # [權重] 最終進化之 AI 模型大腦
   7 ├── pretrained_hunter.zip     # [權重] 模仿人類行為的初期模型
   8 ├── human_demo/               # [數據] 存放所有人類操作錄製檔 (.npz)
   9 └── logs/                     # [日誌] 訓練過程數據 (TensorBoard 使用)
```
<br>
<br>

