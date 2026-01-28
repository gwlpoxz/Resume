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
# [web手寫數字辨識](https://github.com/gwlpoxz/mnist-web-app)

![圖片名稱](https://github.com/gwlpoxz/Resume/blob/main/mnist.png)
<br>
__結合deep Learning、computer vision、web開發的專案，<br>
透過訓練卷積神經網路CNN，並使用 **Flask** 搭建後端 API來辨識手寫數字，<br>
利用簡易互動式web介面，使用者可以即時塗鴉書寫 0-9 的數字，<br>
系統就會透過後端的 PyTorch模型進行即時分類就能辨識結果。__
<br>
+ 核心技術
+ 深度學習框架: PyTorch
+ 後端框架: Flask (Python)
+ 前端技術: HTML5 Canvas, CSS3, JavaScript
+ 圖像處理: Pillow (PIL), Torchvision__

```text
mnist-web-app/
├── app.py                # Flask 後端主程式
├── train.py              # CNN 模型訓練腳本
├── mnist_cnn.pth         # 訓練完成的模型權重檔
├── templates/            # 存放 HTML 檔案
│   └── index.html        # 前端網頁主體
└── static/               # 存放 CSS 與 JS 靜態檔案
    ├── style.css         # 網頁樣式 (對應你的 staticstyle.css)
    └── main.js           # 畫布互動與 API 呼叫邏輯
```


