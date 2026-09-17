數學探險島平台 — 正式 GitHub Pages 發布包
================================================

你目前的 Repository：
  multiplication-adventure

建議改名為：
  username.github.io

其中 username 必須換成你的 GitHub 使用者名稱。

一、Repository 重新命名
-----------------------
GitHub Repository：
Settings -> General -> Repository name

將：
  multiplication-adventure

改成：
  username.github.io

例如 GitHub 使用者名稱若是 wisely：
  wisely.github.io

重新命名後，請確認本發布包的所有檔案位於 Repository 根目錄。

二、正式目錄
------------
username.github.io/
├── index.html
├── about.html
├── projects.html
├── contact.html
├── README_DEPLOY.txt
└── math/
    ├── index.html
    ├── manifest.json
    ├── service-worker.js
    ├── icons/
    │   ├── icon-192.png
    │   ├── icon-512.png
    │   ├── icon-maskable-512.png
    │   └── apple-touch-icon.png
    ├── docs/
    │   ├── development-release-guide.png
    │   ├── installation-overview.png
    │   ├── install-ios-ipados.png
    │   ├── install-android.png
    │   └── install-desktop.png
    ├── multiplication/
    │   └── index.html
    ├── division/
    │   └── index.html
    └── fractions/
        └── index.html

三、GitHub Pages 設定
--------------------
Repository -> Settings -> Pages

Build and deployment：
  Source: Deploy from a branch
  Branch: main
  Folder: /(root)

正式網址：
  https://username.github.io/

數學探險島：
  https://username.github.io/math/

乘法探險島：
  https://username.github.io/math/multiplication/

四、PWA 安裝
------------
請從：
  https://username.github.io/math/

使用 Safari 開啟，再：
  分享 -> 加入主畫面 -> 加入

不要從 multiplication 子頁單獨建立另一個 App。
數學探險島是一個平台型 PWA，未來乘法、除法與分數都由同一個主畫面入口進入。

五、PWA Scope
-------------
/math/service-worker.js
只控制：
  /math/

不會控制：
  /
  /about.html
  /projects.html
  /contact.html

六、版本更新
------------
大型更新時請修改：
  /math/service-worker.js

裡面的 CACHE_NAME，例如：
  math-explorer-island-platform-v1
改成：
  math-explorer-island-platform-v2

瀏覽器在 Service Worker activate 時會清除舊平台快取。

七、說明圖
----------
開發 / 發布說明：
  /math/docs/development-release-guide.png

跨平台安裝總覽：
  /math/docs/installation-overview.png

Apple：
  /math/docs/install-ios-ipados.png

Android：
  /math/docs/install-android.png

Windows / macOS：
  /math/docs/install-desktop.png

安裝步驟也已直接整合在：
  /math/index.html

八、目前內容
------------
乘法：
  已開放，使用乘法探險島 v17

除法：
  準備中

分數：
  準備中


九、品牌視覺 v4
---------------
平台 PWA：
  大島嶼 + 羅盤 + 通往不同區域的小路 + 紫色魔法探險精靈

乘法：
  名稱改為「乘法工坊」
  視覺包含冒煙煙囪、齒輪、× 立牌與工坊版小精靈
  原乘法 v17 教學核心與學習紀錄邏輯保留

除法：
  「除法海灣」視覺加入可愛鯨魚

分數：
  「分數森林」視覺加入蘋果樹

網站資產：
  /math/assets/platform/
  /math/assets/multiplication/
  /math/assets/division/
  /math/assets/fractions/

PWA 主圖示已改為平台圖示，不再使用乘法 × 作為主 App 識別。


十、v5 介面修正
--------------
平台首頁：
  Hero 改為「浮動木牌 / 小看板」樣式，不再以大白卡覆蓋探險地圖。

乘法工坊：
  Hero 改為木牌風標題 + 較小副標，不再以大白卡遮住角色與工坊場景。

文案風格：
  獎勵、提示與勳章名稱改為工坊語言，例如：
  - 連續完成
  - 工坊徽章
  - 作品完成
  - 修正完成


十一、v6 視覺修正
----------------
- 平台首頁移除重複訊息白框，只保留浮動木牌標題。
- 乘法工坊 Hero 移除覆蓋場景的白色副標框，只保留木牌風標題；副標移到圖下方。
- 跨平台安裝總覽與電腦安裝圖解已改為數學探險島世界觀版本。

十二、v7 擴充
-------------
- Apple / Android 安裝圖改為「數學探險島」世界觀獨立圖解。
- 乘法工坊 Toast、工坊徽章、微鼓勵與關卡外觀進一步工坊化。
- 除法海灣與分數森林改為正式入口樣板頁，平台首頁可點入預覽。


十三、v8 世界觀統一
------------------
平台首頁：
  使用已確認的「數學探險島完整主圖」，不再疊加任何額外標題框或說明框。

乘法工坊進度：
  原「探險地圖」改為「工坊進度 / 工坊成長圖」。

工作站名稱：
  Lv.1 🔧 暖身工作台
  Lv.2 ⚙️ 進位練習台
  Lv.3 🧩 雙位組裝區
  Lv.4 🔩 連續進位站
  Lv.5 🏗️ 部分積組裝線
  Lv.6 🎯 精準校準室
  Lv.7 🏆 工匠挑戰室

用語：
  關卡 -> 工作站
  解鎖 -> 啟用
  探險地圖 -> 工坊進度

v8.1：以原始 v8 為唯一基底，只修正四項
-----------------------------------------
1. 獎勵訊息的小精靈圖示不再覆蓋前方文字。
2. 「自己來」改名為「自我挑戰」。
3. 修正乘數只有 1 位時，直式自我挑戰不顯示粉紅乘數與黃色被乘數焦點。
4. 返回數學探險島後再進入乘法工坊，保留：
   被乘數、乘數、被乘數位數、乘數位數、動畫速度、
   介面、資訊模式、音效、教學輔助。
未更換任何 v8 圖片、場景或品牌視覺。

v8.2
----
1. 獎勵訊息維持上下排列，但改用真正的 IMG 顯示小精靈頭像：
   小精靈在上、讚賞文字在下。
2. 新增「↺ 重置設定」按鈕。
   重置內容：
   - 被乘數 / 乘數
   - 被乘數位數 / 乘數位數
   - 動畫速度
   - 介面（兒童化）
   - 資訊（孩子模式）
   - 音效（開）
   - 教學輔助（自動）
   不清除學習紀錄、徽章與工作站進度。
3. 所有圖片資產維持 v8.1 原樣。


v8.3
----
1. 套用新的平台首頁主圖：修正數學探險島小精靈多餘第三觸手腳。
2. 套用新的乘法工坊上方主圖：改為工坊內部配置圖。
3. 新增 `math/docs/v8.3-stability-checklist.md` 供穩定性巡檢使用。
4. Service Worker 快取版號更新為 `platform-v8-3`。


v8.3.1
------
1. 修正 v8.3 誤將首頁的乘法工坊入口圖一併替換。
2. 恢復首頁／平台中的乘法工坊入口圖為 v8.2 原始版本。
3. 乘法工坊頁首上方圖維持使用工坊內部配置圖，改用獨立資產 `workshop-interior.webp`。
4. Service Worker 快取版號更新為 `platform-v8-3-1`。


V9.0
----
基底：V8.3.1（穩定版）
1. 精準錯誤診斷：一次只指出目前最值得修的一步，並以中文教師判讀顯示。
2. 繼續上次練習：保存工作站／自我挑戰模式與練習位置，不保存半成品答案。
3. 重置設定會一併清除「上次練習位置」，但不清除學習紀錄、徽章或工作站進度。
4. 基本觸控／鍵盤輸入優化：數字自動前進、空格 Backspace 返回上一格、Enter 檢查、最小必要捲動。
5. 不加入特殊手機鍵盤重排與橫向模式專用版面。
6. 圖像資產完全沿用 V8.3.1。


v9.0.1
------
1. 移除按「檢查」後的錯誤格額外高亮；診斷改為下方文字說明。
2. 原本教學輔助的色彩提示維持不變。
3. 診斷文字不再依賴「綠框」指示。
4. 補強進位錯誤判讀：47 × 6 輸入 242 可判讀為「進位錯誤」。
5. Service Worker 快取版號更新為 platform-v9-0-1。


v9.1
----
1. 新增「我的學習摘要」：最近第一次答對率、主要錯誤、最近表現、文字型練習建議。
2. 練習建議不綁工作站，不會因工作站尚未啟用而產生矛盾。
3. 工作站卡片新增：未啟用、已啟用、練習中、已完成／再次練習中等狀態。
4. 新增工坊整體進度 X/7 與進度條。
5. 第一次完成工作站時，保留原單題成功鼓勵，之後再播放較大型工作站完成慶祝。
6. 已完成工作站重做時不再觸發大型完成慶祝。
7. Service Worker 快取版號更新為 platform-v9-1。


v9.2
----
1. about.html：套用使用者核定的「數學探險島理念」版本。
2. contact.html：套用使用者核定的 Email 聯絡版本，家長介面不顯示 GitHub / GitHub Issues。
3. math/docs/development-release-guide.png：換成使用者提供的新版本，統一小精靈風格並使用實際網址 sakuchi0309.github.io。
4. 其餘乘法工坊核心功能與圖片資產不變。
5. Service Worker 快取版本更新為 platform-v9-2。

v9.2.1
------
1. 套用新版 about.html（使用者提供內容）。
2. 可見英文世界觀名稱統一為「Math Adventure Island」。
3. contact.html footer 同步改為 Math Adventure Island。
4. Service Worker cache version 更新為 platform-v9-2-1。
