# 潘冠伶(Gwen Pan)

　●Education:南臺科技大學 / 資訊管理系<br>
　●Location: Tainan City<br>
　●E-mail: gwenlyn.pan@gmail.com<br>
　●Mobile: 0908-780-157<br>
---

### 專業技能

　●使用並基礎了解後端運作 PHP,資料庫及 MySQL 語法。<br>
　●MySQL分析繪製E-R Model、規劃Table Schema，以及利用SQL關聯式資料庫進行資料查詢及處理。<br>
　●Visual studio 利用C#語言撰寫Windows Forms App(.Net Framework)。<br>
　●使用爬蟲更新資料庫內容。<br>


***
### 作品集

#### 股價查詢系統

![圖片名稱](圖片url)

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


