# MICROSYS PPE 智慧工地安全平台

## 項目概述

這是一個專為封閉式網路環境設計的智慧工地安全平台模板，基於 AdminLTE 框架開發，提供完整的 PPE（個人防護裝備）管理功能。

## 主要功能

- 📊 **儀錶板** - 即時監控工地安全狀況
- 👥 **人員管理** - 工地人員進出管理
- 🚗 **車輛管理** - 工地車輛進出追蹤
- ⏰ **出勤管理** - 人員出勤記錄
- 🚪 **門禁管理** - 安全門禁控制
- 📋 **看板管理** - 工地資訊看板
- 🔐 **權限管理** - 系統權限控制

## 技術架構

- **前端框架**: AdminLTE 3.2
- **CSS 框架**: Bootstrap 4.6.2
- **JavaScript 庫**: jQuery 3.6.0, Chart.js 3.9.1
- **圖標庫**: FontAwesome 5.15.4
- **主題**: 支援明暗主題切換

## 目錄結構

```
microsys-template/
├── css/                    # CSS 樣式文件
│   ├── adminlte.min.css   # AdminLTE 主樣式
│   └── all.min.css        # FontAwesome 圖標樣式
├── js/                     # JavaScript 文件
│   ├── jquery.min.js      # jQuery 庫
│   ├── bootstrap.bundle.min.js  # Bootstrap 組件
│   ├── adminlte.min.js    # AdminLTE 功能
│   └── chart.min.js       # Chart.js 圖表庫
├── webfonts/              # 字體文件
│   ├── fa-brands-400.woff2
│   ├── fa-regular-400.woff2
│   └── fa-solid-900.woff2
├── img/                   # 圖片資源
├── dashboard.html         # 主儀錶板頁面
├── login.html            # 登入頁面
└── README.md             # 項目說明文件
```

## CDN 轉本地資源記錄

### 修改日期
2025年1月

### 修改原因
為適應封閉式網路環境，將所有外部 CDN 資源轉換為本地資源。

### 轉換詳情

#### 1. CSS 文件轉換
| 原始 CDN 路徑 | 本地路徑 | 說明 |
|--------------|----------|------|
| `https://cdn.jsdelivr.net/npm/admin-lte@3.2/dist/css/adminlte.min.css` | `css/adminlte.min.css` | AdminLTE 主樣式 |
| `https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@5.15.4/css/all.min.css` | `css/all.min.css` | FontAwesome 圖標樣式 |

#### 2. JavaScript 文件轉換
| 原始 CDN 路徑 | 本地路徑 | 說明 |
|--------------|----------|------|
| `https://cdn.jsdelivr.net/npm/jquery@3.6.0/dist/jquery.min.js` | `js/jquery.min.js` | jQuery 核心庫 |
| `https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/js/bootstrap.bundle.min.js` | `js/bootstrap.bundle.min.js` | Bootstrap 組件 |
| `https://cdn.jsdelivr.net/npm/admin-lte@3.2/dist/js/adminlte.min.js` | `js/adminlte.min.js` | AdminLTE 功能 |
| `https://cdn.jsdelivr.net/npm/chart.js@3.9.1/dist/chart.min.js` | `js/chart.min.js` | Chart.js 圖表庫 |

#### 3. 字體文件下載
| 字體文件 | 本地路徑 | 說明 |
|----------|----------|------|
| `fa-brands-400.woff2` | `webfonts/fa-brands-400.woff2` | FontAwesome 品牌圖標 |
| `fa-regular-400.woff2` | `webfonts/fa-regular-400.woff2` | FontAwesome 常規圖標 |
| `fa-solid-900.woff2` | `webfonts/fa-solid-900.woff2` | FontAwesome 實心圖標 |

#### 4. 修改的文件
- `dashboard.html` - 更新所有 CDN 路徑為本地路徑
- `login.html` - 更新所有 CDN 路徑為本地路徑
- `css/all.min.css` - 優化字體路徑，只保留 woff2 格式

### 優化措施

1. **字體優化**: 只保留 woff2 格式字體文件，減少文件大小
2. **路徑統一**: 所有資源使用相對路徑，便於部署
3. **版本固定**: 使用特定版本的庫文件，確保穩定性

## 部署說明

### 環境要求
- 現代瀏覽器（Chrome 60+, Firefox 55+, Safari 12+, Edge 79+）
- 支援 JavaScript 和 CSS3
- 無需伺服器端支援（純前端應用）

### 部署步驟

1. **下載項目**
   ```bash
   # 將整個項目目錄複製到目標環境
   ```

2. **驗證文件完整性**
   - 確認 `css/` 目錄包含所有樣式文件
   - 確認 `js/` 目錄包含所有 JavaScript 文件
   - 確認 `webfonts/` 目錄包含所有字體文件

3. **測試功能**
   - 打開 `login.html` 測試登入頁面
   - 打開 `dashboard.html` 測試主功能
   - 確認主題切換功能正常
   - 確認圖表顯示正常

### 注意事項

- 所有資源已本地化，無需網路連接
- 支援離線使用
- 主題設定會保存在瀏覽器本地存儲中
- 建議在 HTTPS 環境下部署以確保安全性

## 功能特色

### 🎨 主題系統
- 支援明暗主題切換
- 主題設定自動保存
- 響應式設計

### 📊 數據可視化
- 柱狀圖顯示人員分布
- 圓餅圖顯示比例統計
- 即時數據更新

### 🔔 通知系統
- 即時警報通知
- 安全帽檢測提醒
- 危險區域警告

### 📱 響應式設計
- 支援桌面和移動設備
- 自適應佈局
- 觸控友好界面

## 版本資訊

- **當前版本**: 1.0.0
- **最後更新**: 2025年1月
- **相容性**: 現代瀏覽器

## 授權資訊

Copyright © 2025 Microsys Information Co., Ltd. All rights reserved.

---

## 聯絡資訊

如有問題或建議，請聯繫開發團隊。

---

## 更新記錄

### 2025年1月 - 主題切換功能修復

#### 修復內容
- **問題**: 主題切換按鈕失效，無法正常切換明暗主題
- **原因**: JavaScript 變數作用域問題和事件綁定時機問題
- **解決方案**:
  1. 將圖表變數改為全局變數，避免作用域問題
  2. 使用 `DOMContentLoaded` 事件確保 DOM 完全載入後再綁定事件
  3. 添加錯誤處理和調試信息
  4. 重新下載 Chart.js 文件確保完整性

#### 修改的文件
- `dashboard.html` - 修復主題切換 JavaScript 代碼
- `login.html` - 統一主題切換事件綁定方式
- `test-theme.html` - 新增主題切換功能測試頁面

#### 測試方法
1. 打開 `test-theme.html` 進行基本功能測試
2. 打開 `dashboard.html` 測試完整功能
3. 打開 `login.html` 測試登入頁面主題切換
4. 檢查瀏覽器控制台是否有錯誤信息

#### 驗證要點
- ✅ 主題切換按鈕正常響應
- ✅ 頁面顏色正確切換
- ✅ 按鈕圖標正確更新
- ✅ 主題設定在頁面重新整理後保持
- ✅ 圖表顏色隨主題切換而更新
