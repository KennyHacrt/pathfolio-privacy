# Privacy Policy — Pathfolio

**Last updated:** November 15, 2026

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

### Flight records and boarding-pass images (on your device)

Flight records (airports, departure date and optional flight number) stay on
your phone. Optional flight suggestions are off by default. If you enable them,
Pathfolio compares your latest permitted location checks, including a foreground
check when you reopen the app without Exploring, and stores a last known location
on your phone to propose a possible flight for your confirmation. This does not
enable a new always-running flight tracking service. Suggestions do not become
confirmed flights automatically.

On iOS, boarding-pass or booking images selected for flight recognition are read
locally with Apple Vision. They are not sent to our server or DeepSeek. Temporary
copies received through the flight share flow are deleted after processing; your
original Photos images are not deleted. Flight JSON/Google Timeline files are read
locally only when you select them. Flight data is not included in cloud exploration
backups. You can export a local JSON backup, delete individual flights, and choose
whether to share a flight image or backup with another app; the receiving app's
policy then applies. Turning off location-based flight suggestions clears the
stored last flight-location fix; your existing flight records remain until deleted.

### Friends and what you choose to share

Friends features need a Google or Apple sign-in. Your display name, short bio and friend code are visible to people you add as friends, and anyone who has your exact friend code can find your display name to send a request.

Nothing is shared automatically. When you share a place, its name, coordinates, note and source links are uploaded for your accepted friends. When you share a route, you pick the dates and how it is shown:

- **Streets only** uploads the street cells you walked in those dates, plus its distance, countries and regions.
- **Full route** also uploads the time-ordered GPS track for those dates, so friends can replay the order you walked.

The GPS track is otherwise kept on your phone and is never part of a backup. For each shared place you can also pick photos to show. None are shown by default, and only the photos you pick are uploaded. They are readable only by you and your accepted friends. You can delete a shared route, remove a photo or remove a friend at any time. Deleting your account deletes all of this.

You can also **send** a place or a route to chosen friends. Only the friends you pick can see it, and you can only send to accepted friends. A sent place carries its name, coordinates, category, Instagram/Threads post links and its cover photo; your note and other photos are not sent. A sent route is uploaded only when you send it and does not appear on your profile. These shares hold no free text or other links. We keep each share, who sent it to whom, when, and when it was read, so the receiver can see it later. You can unsend a share at any time. Deleting your account deletes the shares and cover photos you sent.

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
| Supabase | Optional authentication, backup of visited cells, and the profile, places, routes, photos and sent shares you choose to share (row-level security limits each to you and, for shared items, your accepted friends or the friends you send them to) |
| Google (Sign-In, Play, AdMob) | Optional sign-in, purchases, rewarded ads |
| Apple (App Store, Sign in with Apple when required) | iOS purchases and sign-in |
| RevenueCat | Purchase entitlement |
| OpenStreetMap / tile provider / Nominatim | Map tiles and optional place search |
| DeepSeek | Suggests a place from shared posts' captions, cover images, and screenshots or photos you add |

Each provider processes data under their own privacy policies.

## Data Retention & Deletion

- **On the phone:** trail, pins and badges stay until you clear app data or uninstall.
- **In the cloud:** optional backups stay while your account is active.
- **Delete account:** Settings → Delete account & cloud data. This removes your cloud backup, shared places, routes, photos, sent shares and their cover photos, and account. The map on this phone is kept. You can also email us (see Contact).

Purchase records may be kept by Google Play, the App Store and RevenueCat as required for billing. Encrypted infrastructure backups at Supabase expire within about 30 days.

## Children's Privacy

Pathfolio is not directed at children under 13. We do not knowingly collect personal information from children.

## Changes to This Policy

We may update this policy from time to time. The "Last updated" date at the top will change when we do.

## Contact

**Email:** [lee.mh.kenny@gmail.com](mailto:lee.mh.kenny@gmail.com)

---

## 隱私權政策 — Pathfolio（繁體中文摘要）

**最後更新：** 2026 年 11 月 15 日

Pathfolio 是旅行日記與地圖 App。GPS 會在手機上把你走過的街道畫成迷霧地圖。**探索紀錄預設只存在這支手機。** 只有你用 Google 登入並點「立即備份」，或開啟「自動備份」（預設關閉，離開 App 時上傳）時，才會上傳到雲端（Supabase）。免費使用者可選擇看獎勵廣告，預覽鎖定國家 24 小時。國家解鎖與 Premium 透過 Google Play / App Store 與 RevenueCat 處理。

- **精確位置：** 點「開始探索」後（含背景定位與持續通知）以約 40×20 公尺的格子記錄足跡。模擬定位會被忽略。
- **航班（選用）：** 航班的機場、日期和航班編號只存在手機。位置建議預設關閉；開啟後會比較取得的位置，包括未開啟探索時重新進入 App 的前景定位，並保留上一筆位置來建議可能的航班，由你確認。這不會啟動另一個持續運作的飛行追蹤服務。iOS 的登機證／訂票圖片以 Apple Vision 在手機辨識，不傳給伺服器或 DeepSeek；系統分享流程的暫存圖片在處理後刪除，原本的相簿圖片保留。選取的航班 JSON／Google Timeline 檔案也只在手機處理。航班不包含在雲端足跡備份，你可匯出 JSON 備份或主動分享航線圖片；接收 App 的政策適用。關閉航班位置建議會清除上一筆航班定位，既有航班則保留至你刪除。
- **備份（選用）：** Google 登入取得 email 與使用者 ID；備份內容為格子雜湊、國家代碼與首次造訪時間。
- **貼文釘選：** 分享 Instagram／Threads 貼文、截圖或相片到 App 後，App 會把貼文文字、公開封面圖片和你加入作線索的截圖／相片（不含你的位置或帳號資料）經我們的伺服器交給 DeepSeek（伺服器位於中國）推測地點，再向 OpenStreetMap 搜尋；從圖片認出的地點只作建議，由你確認。文字和圖片不會保存在伺服器，只記錄每日次數以防濫用。
- **朋友（選用，需登入）：** 朋友可看到你的顯示名稱、簡介和好友代碼；持有你完整好友代碼的人可搜尋到你的顯示名稱以送出邀請。只有你主動分享的內容才會上傳：地點（名稱、座標、備註、來源連結）；路線（你選擇日期，「只顯示走過的街區」上傳街區格子，「完整路線」另外上傳該段日期的有序 GPS 軌跡）；每個地點由你逐張挑選的相片（預設不分享，僅你和已加入的朋友可看）。你可隨時刪除，刪除帳號時全部移除。
- **傳送給朋友（選用）：** 你可把地點或路線傳給選定的朋友，只有收件人看得到，而且只能傳給已加入的朋友。傳送的地點包括名稱、座標、類別、Instagram／Threads 貼文連結和封面相；你的備註和其他相片不會傳出。路線在傳送時才上傳，不會出現在你的個人檔案。分享中沒有自由文字或其他連結。我們保存每則分享、寄件人和收件人、時間及已讀時間。你可隨時收回，刪除帳號時你傳出的分享和封面相會一併刪除。
- **廣告：** 只有你主動看的獎勵廣告（AdMob）；地圖上沒有橫幅或插頁廣告。
- **刪除帳號：** 設定 → 刪除帳號與雲端資料。雲端備份及分享的地點、路線、相片和傳出的分享會刪除，手機上的地圖會保留。
- **我們不出售個人資料，也不用足跡來投放廣告。**

如有疑問，請來信：**[lee.mh.kenny@gmail.com](mailto:lee.mh.kenny@gmail.com)**

