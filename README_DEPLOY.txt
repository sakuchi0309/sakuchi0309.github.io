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
