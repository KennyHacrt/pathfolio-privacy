# Privacy Policy — Pathfolio

**Last updated:** November 9, 2026

Kenny Lee ("we", "us") operates the mobile application **Pathfolio**. This page explains how we handle information when you use our app.

## Summary

Pathfolio is a travel diary and map. GPS paints the streets you walk as a fog-of-war trail on your phone. **Exploration is recorded on-device by default.** You upload a backup to our cloud (Supabase) only if you sign in with Google and tap **Back up**, or turn on **Back up automatically** (off by default), which uploads whenever you leave the app. Free users may watch an optional rewarded ad to peek at a locked country for 24 hours. Optional in-app purchases (per-country unlocks and Premium) go through Google Play or the App Store and RevenueCat.

## Information We Collect

### Precise location (on your device)

When you tap **Start exploring**, Pathfolio uses GPS (including **background location** while exploring, with a persistent notification) to record which ~40×20 m street cells you visited. Those cells are stored in a local database on your phone as geohash codes plus a country code. The map uses this to lift fog and show progress.

Location is **not** sent to our servers unless you choose **Back up** or turn on **Back up automatically**. Fake / mock GPS fixes are ignored. A VPN does not change GPS.

You can stop exploring at any time. Uninstalling the app, or clearing app data, removes the local trail.

### Optional account and backup

If you sign in with **Google**, we receive your **email address** and a unique user identifier. We use this only to authenticate you.

When you tap **Back up** (or automatically, if you turned that on), we upload visited cell hashes, country codes, and first-seen timestamps to **Supabase** so you can restore them. We do not receive photos from this backup in the current version.

### Friends and what you choose to share

Friends features need a Google or Apple sign-in. Your display name, short bio and friend code are visible to people you add as friends, and anyone who has your exact friend code can find your display name to send a request.

Nothing is shared automatically. When you share a place, its name, coordinates, note and source links are uploaded for your accepted friends. When you share a route, you pick the dates and how it is shown:

- **Streets only** uploads the street cells you walked in those dates, plus its distance, countries and regions.
- **Full route** also uploads the time-ordered GPS track for those dates, so friends can replay the order you walked.

The GPS track is otherwise kept on your phone and is never part of a backup. For each shared place you can also pick photos to show. None are shown by default, and only the photos you pick are uploaded. They are readable only by you and your accepted friends. You can delete a shared route, remove a photo or remove a friend at any time. Deleting your account deletes all of this.

### Pins from shared posts (on your device)

If you share an Instagram post or Reel (or another link), or screenshots and photos, into Pathfolio, the app reads the caption or link preview on your phone to guess a place, then searches **OpenStreetMap Nominatim**. Pins and source links stay in local storage until you remove them. Place search sends only the place name you search for, not your GPS trail. To suggest place names, the app sends the posts' caption text, their public cover images, and any screenshots or photos you add as clues (not your location or your account details) to our server, which asks **DeepSeek** (servers in China). A place recognised from the image is shown as a suggestion for you to confirm. We keep only a daily request count per account (or a one-way hash of the network address for guests) to limit use; captions and pictures are not stored on our server. Pictures you add as clues are kept on your phone with the pin.

### Device, ads, and purchases

- **Google AdMob** may collect device identifiers (such as the advertising ID) when you choose to watch a rewarded ad. Pathfolio does not show banner or interstitial ads over the map.
- **Google Play Billing / App Store / RevenueCat** process Premium subscriptions and one-time country unlocks. We receive entitlement status, not your card details.
- **Map tiles** load from the configured tile provider (OpenStreetMap in development). Tile requests use your approximate map view, not your stored trail.

### Permissions

| Permission | Purpose |
|------------|---------|
| Precise / coarse location | Paint the streets you walk |
| Background location | Keep painting after you leave the app while Exploring is on |
| Foreground service / notifications | Show the persistent "exploring" notification |
| Ignore battery optimization (optional) | Stop some Android skins from killing GPS |
| Internet | Optional backup, map tiles, place search, ads, purchases |
| Advertising ID (Android) | AdMob when you watch a rewarded ad |

## How We Use Information

- Draw your fog-of-war map and country / region progress
- Optional cloud backup and restore
- Optional rewarded-ad peeks and paid unlocks
- Pin places you save from shared posts
- Show friends the places, routes and photos you choose to share

We do **not** sell your personal data. We do not use your trail to show ads.

## Data Sharing

| Provider | Purpose |
|----------|---------|
| Supabase | Optional authentication, backup of visited cells, and the profile, places, routes and photos you choose to share (row-level security limits each to you and, for shared items, your accepted friends) |
| Google (Sign-In, Play, AdMob) | Optional sign-in, purchases, rewarded ads |
| Apple (App Store, Sign in with Apple when required) | iOS purchases and sign-in |
| RevenueCat | Purchase entitlement |
| OpenStreetMap / tile provider / Nominatim | Map tiles and optional place search |
| DeepSeek | Suggests a place from shared posts' captions, cover images, and screenshots or photos you add |

Each provider processes data under their own privacy policies.

## Data Retention & Deletion

- **On the phone:** trail, pins and badges stay until you clear app data or uninstall.
- **In the cloud:** optional backups stay while your account is active.
- **Delete account:** Settings → Delete account & cloud data. This removes your cloud backup, shared places, routes and photos, and account. The map on this phone is kept. You can also email us (see Contact).

Purchase records may be kept by Google Play, the App Store and RevenueCat as required for billing. Encrypted infrastructure backups at Supabase expire within about 30 days.

## Children's Privacy

Pathfolio is not directed at children under 13. We do not knowingly collect personal information from children.

## Changes to This Policy

We may update this policy from time to time. The "Last updated" date at the top will change when we do.

## Contact

**Email:** [lee.mh.kenny@gmail.com](mailto:lee.mh.kenny@gmail.com)

---

## 隱私權政策 — Pathfolio（繁體中文摘要）

**最後更新：** 2026 年 11 月 9 日

Pathfolio 是旅行日記與地圖 App。GPS 會在手機上把你走過的街道畫成迷霧地圖。**探索紀錄預設只存在這支手機。** 只有你用 Google 登入並點「立即備份」，或開啟「自動備份」（預設關閉，離開 App 時上傳）時，才會上傳到雲端（Supabase）。免費使用者可選擇看獎勵廣告，預覽鎖定國家 24 小時。國家解鎖與 Premium 透過 Google Play / App Store 與 RevenueCat 處理。

- **精確位置：** 點「開始探索」後（含背景定位與持續通知）以約 40×20 公尺的格子記錄足跡。模擬定位會被忽略。
- **備份（選用）：** Google 登入取得 email 與使用者 ID；備份內容為格子雜湊、國家代碼與首次造訪時間。
- **貼文釘選：** 分享 Instagram／Threads 貼文、截圖或相片到 App 後，App 會把貼文文字、公開封面圖片和你加入作線索的截圖／相片（不含你的位置或帳號資料）經我們的伺服器交給 DeepSeek（伺服器位於中國）推測地點，再向 OpenStreetMap 搜尋；從圖片認出的地點只作建議，由你確認。文字和圖片不會保存在伺服器，只記錄每日次數以防濫用。
- **朋友（選用，需登入）：** 朋友可看到你的顯示名稱、簡介和好友代碼；持有你完整好友代碼的人可搜尋到你的顯示名稱以送出邀請。只有你主動分享的內容才會上傳：地點（名稱、座標、備註、來源連結）；路線（你選擇日期，「只顯示走過的街區」上傳街區格子，「完整路線」另外上傳該段日期的有序 GPS 軌跡）；每個地點由你逐張挑選的相片（預設不分享，僅你和已加入的朋友可看）。你可隨時刪除，刪除帳號時全部移除。
- **廣告：** 只有你主動看的獎勵廣告（AdMob）；地圖上沒有橫幅或插頁廣告。
- **刪除帳號：** 設定 → 刪除帳號與雲端資料。雲端備份及分享的地點、路線和相片會刪除，手機上的地圖會保留。
- **我們不出售個人資料，也不用足跡來投放廣告。**

如有疑問，請來信：**[lee.mh.kenny@gmail.com](mailto:lee.mh.kenny@gmail.com)**
