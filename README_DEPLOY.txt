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
