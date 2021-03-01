## React：台灣即時天氣查詢 App
一個結合 React 前端開發技術、串接中央氣象局 API 的台灣即時天氣查詢系統，除了能夠立即查詢各縣市天氣狀況，也提供溫度、降雨量、風速及天氣描述等詳細資料以供用戶參考。
- [Demo](https://sophiebetough.github.io/weather-in-taiwan-app/)
- [中央氣象局 API](https://opendata.cwb.gov.tw/dist/opendata-swagger.html#/)

![image](放上照片)

### 核心功能
- 天氣查詢功能，即時顯示溫度、天氣描述、降雨量及風速等數據。
- 提供台灣各縣市的天氣即時狀態、透過選取功能，掌握各地天氣狀態。
- 支援深色主題模式（Dark Mode)，根據中央氣象局提供的日出和日落資料，來判斷當前主題模式。
- 切換頁面功能，讓用戶透過按鈕進行網頁的變換。
- 保存用戶偏好設定的地區資訊功能，也設置 `localStorage` 資料的時效時間。
- 網頁可下載到手機裝置，作為 Web App 安裝在手機上。

![image](https://github.com/sophiebetough/weather-in-taiwan-pwa/blob/170a9a8dfa97debf83ec395bad670d9ad920ae74/public/dark-mode-demo.png)

### 使用技術
- 以 React 搭配中央氣象局 API 資料，建立台灣即時天氣查詢系統。
- 以 JSX 語法撰寫元件，並搭配 styled-components 進行排版。
- 使用 function component 及 hooks 管理狀態。
- 啟用 PWA 功能，將網頁變成手機 Web App。
- 安裝 normalize.css，重置各瀏覽器使基本樣式一致。
- 套用 dayjs 處理處理跨瀏覽器時間問題。
- 導入 Prettier、ESLint 統一程式碼格式及檢查語法。

### 專案結構
- /src
    - /components
        - WeatherIcon.js
    - /hooks
        - useWeatherAPI.js
    - /pages
        - WeatherCard.js
        - WeatherSetting.js
    - /utils
        - helpers.js
        - sunrise-sunset.json
    - /images：images that the project needs
    - App.js
    - App.css
    - index.js
    - index.css
