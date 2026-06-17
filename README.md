# 香港音游CheckMaiWay

香港街機音樂遊戲地圖與出行檢查工具。網站針對香港可遊玩的街機音遊店舖，整理店舖位置、機種分類、營業時間、收藏、地圖連結，以及由主要口岸 / 西九龍高鐵站 / 香港國際機場出發與返程的交通資訊。

目前版本：`v1.1.10`

網站：

- Cloudflare Pages: <https://hk-otoge-checkmaiway.pages.dev/>
- GitHub Pages: <https://littlestarprpr.github.io/hk-otoge-CheckMaiWay/>

## 功能

- 香港音遊機廳地圖總覽，支援桌面與手機瀏覽。
- 歡迎頁顯示總統計、機種分類、資料來源與免責提示。
- 地圖縮放 / 移動時，列表會同步顯示目前地圖範圍內的機廳。
- 依起點自動置頂最近 / 路費最低機廳，並以綠色呼吸環標示。
- 店舖卡片顯示名稱、地區、地址、人氣值、營業時間、機種、更新來源與地圖連結。
- 每間店提供 Apple 地圖、Google 地圖、BEMANI CN、ZIv 連結。
- 可收藏常去店舖，收藏資料儲存在本機瀏覽器。
- 支援亮色與 OLED 純黑暗黑模式。
- 支援起點 / 終點選擇，估算去程交通費與理論最快路線時間。
- 支援返程估算，並分開顯示口岸關閉紅線與港鐵末班車紅線。
- 口岸紅線會預留至少 30 分鐘過關緩衝。
- 如口岸關閉紅線早於港鐵末班車紅線，頁面只顯示最終有效的口岸紅線。
- 香港國際機場起點會獨立顯示普通遊客價格、套用優惠後價格及優惠所需條件。
- 選定起點與店舖後，頁面與地圖會以港鐵線路色塊和小徽標顯示相關路線。

## 機種分類

SEGA 系：

- maimaiDX
- CHUNITHM

KONAMI 系：

- beatmania IIDX
- SOUND VOLTEX

篩選邏輯：初始狀態顯示全部機種；單點一個機種會只顯示該機種；再點其他機種會進入多選篩選。

## 交通起點

目前支援以下起點：

- 西九龍高鐵站 / 高鐵西九龍口岸
- 羅湖口岸
- 落馬洲支線 / 福田口岸
- 深圳灣口岸
- 香園圍口岸
- 港珠澳大橋香港口岸
- 香港國際機場 / 機場快線機場站

交通費、路線時間、末班車與口岸時間均為公開資料推算。香港國際機場不套用口岸關閉時間，只顯示返程港鐵 / 機場快線末班約束與機場快線班次提示。實際出行請以港鐵、口岸、機場及現場資訊為準。

## 資料來源

主要資料來源包括：

- BEMANI CN
- Zenius-I-vanisher
- MTR 官方 HRRoutes API 與機場快線時間表
- 香港入境事務處口岸辦公時間
- 公開巴士票價資料
- 公開社群與店舖備註資訊

資料生成日期：`2026-06-17`

## 免責

本頁面僅供出行和選店參考。機台數量、版本、營業時間、店舖狀態、票價、路線、口岸安排與現場人流可能隨時變化。出發前請以機廳現場、官方交通及口岸資訊為準。人氣值只表示公開社群熱度，不代表即時排隊人數。

## 部署

本專案是靜態單頁網站，`index.html` 為入口，可部署到：

- Cloudflare Pages
- GitHub Pages
- Netlify
- Vercel Static Project

---

# Hong Kong Otoge CheckMaiWay

A mobile-friendly and desktop-friendly arcade rhythm game map for Hong Kong. The site collects arcade locations, game categories, opening hours, favorites, map links, and transport estimates from major border checkpoints, Hong Kong West Kowloon Station, and Hong Kong International Airport.

Current version: `v1.1.10`

Live site:

- Cloudflare Pages: <https://hk-otoge-checkmaiway.pages.dev/>
- GitHub Pages: <https://littlestarprpr.github.io/hk-otoge-CheckMaiWay/>

## Features

- Overview map for Hong Kong arcade rhythm game locations.
- Welcome screen with total counts, game categories, data sources, and disclaimer.
- Arcade list updates dynamically based on the current map viewport.
- Automatically pins the nearest / lowest-fare arcade for the selected origin with a green pulse highlight.
- Arcade cards show name, district, address, popularity score, opening hours, game availability, source updates, and map links.
- Apple Maps, Google Maps, BEMANI CN, and ZIv links for each arcade.
- Local browser favorites for frequently visited arcades.
- Light mode and OLED pure-black dark mode.
- Origin / destination selector for estimated outbound fare and theoretical fastest route time.
- Return-trip estimate with separate border checkpoint deadline and MTR last-train deadline.
- Border checkpoint deadlines include at least a 30-minute clearance buffer.
- If the border checkpoint closing deadline is earlier than the MTR last-train deadline, only the effective border deadline is shown.
- Hong Kong International Airport shows regular visitor fare, discounted fare, and the required discount conditions separately.
- Selected origin / destination routes show MTR line badges and map route overlays with line reference colors.

## Game Categories

SEGA-side games:

- maimaiDX
- CHUNITHM

KONAMI-side games:

- beatmania IIDX
- SOUND VOLTEX

Filter behavior: all games are shown by default. Selecting one category switches to single-category view; selecting additional categories enables multi-select filtering.

## Supported Origins

- Hong Kong West Kowloon Station / West Kowloon Control Point
- Lo Wu Control Point
- Lok Ma Chau Spur Line / Futian Control Point
- Shenzhen Bay Control Point
- Heung Yuen Wai Control Point
- Hong Kong-Zhuhai-Macao Bridge Hong Kong Port
- Hong Kong International Airport / Airport Express Airport Station

Fare, route time, last-train, and border checkpoint estimates are derived from public data. Hong Kong International Airport is not treated as a border checkpoint; it only shows the MTR / Airport Express last-train constraint and Airport Express frequency note. Check official sources before travel.

## Data Sources

Main sources include:

- BEMANI CN
- Zenius-I-vanisher
- MTR official HRRoutes API and Airport Express timetable
- Hong Kong Immigration Department control point opening hours
- Public bus fare references
- Public community and arcade notes

Data generated on: `2026-06-17`

## Disclaimer

This site is for trip planning and arcade selection reference only. Machine counts, versions, opening hours, arcade status, fares, routes, checkpoint arrangements, and crowd levels may change at any time. Please verify with the arcade, official transport sources, and border checkpoint information before departure. Popularity scores represent public community activity and do not indicate real-time queue length.

## Deployment

This is a static single-page site. `index.html` is the entry point and can be hosted on:

- Cloudflare Pages
- GitHub Pages
- Netlify
- Vercel Static Project
