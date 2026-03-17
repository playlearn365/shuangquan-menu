[README.md](https://github.com/user-attachments/files/26071035/README.md)
# 🍱 基隆市私立雙全幼兒園 — 餐點表自動生成系統

每月一鍵生成幼兒園餐點表，支援下載 Excel 檔案。

## 🌐 線上使用

部署完成後直接開啟網址即可使用，無需安裝任何軟體。

---

## 🚀 部署到 GitHub Pages（5分鐘完成）

### 步驟 1：建立 GitHub Repository

1. 登入 [GitHub](https://github.com)
2. 點擊右上角 **+** → **New repository**
3. Repository name 填入：`shuangquan-menu`（或任何名稱）
4. 設定為 **Public**
5. 點擊 **Create repository**

### 步驟 2：上傳檔案

將以下兩個檔案上傳到 repository：
- `index.html`
- `menu_data.json`

上傳方式：點擊 **Add file** → **Upload files** → 把兩個檔案拖進去 → **Commit changes**

### 步驟 3：開啟 GitHub Pages

1. 進入 repository 頁面
2. 點擊 **Settings**（設定）
3. 左側找到 **Pages**
4. Source 選擇 **Deploy from a branch**
5. Branch 選擇 **main**，資料夾選 **/ (root)**
6. 點擊 **Save**

等待約 1-2 分鐘，網址會出現在 Pages 設定頁面：
```
https://你的GitHub帳號.github.io/shuangquan-menu/
```

---

## 📋 功能說明

| 功能 | 說明 |
|------|------|
| 生成菜單 | 根據年度、月份、季節自動排餐 |
| 每次不同 | 同月份每次點擊都會產生不同排列 |
| 點擊編輯 | 任意格子可直接點擊修改 |
| 下載 Excel | 含完整格式，可直接存檔留存 |
| 列印 | 瀏覽器內建列印，可另存 PDF |

## 📐 排餐規則

- **週一、三、五** 早點：麵點類（米粉/粄條/米苔目/麵食）
- **週二、四** 早點：粥類
- **週二、五** 午餐：麵食或燴飯類
- **週四** 主食：雜糧飯輪替（燕麥/糙米/紫米/地瓜/五穀）
- **週五** 下午：麵包/饅頭等成品
- **冬季** 週四下午：熱甜湯（每週1次）
- **夏季** 週二、四下午：冷甜點（每週2次）

## 🎉 節慶菜單

| 節慶 | 月份 | 特別菜單 |
|------|------|---------|
| 農曆春節前 | 1月第4週 | 圍爐慶團圓火鍋大餐 |
| 中秋節前後 | 8月第3週 | 中秋烤肉拼盤+月餅 |
| 冬至 | 12月第3週 | 冬至湯圓 |

## 📊 資料庫規模

來源：113年、114年全年（共25個月）歷史菜單

| 類別 | 菜品數 |
|------|--------|
| 早點粥類 | 53種 |
| 早點麵點 | 101種 |
| 午餐飯類 | 142種 |
| 午餐麵類 | 93種 |
| 下午甜湯 | 55種 |
| 下午鹹點 | 50種 |
| 下午麵包 | 25種 |

---

## 🔧 本地開發

```bash
# 克隆專案
git clone https://github.com/你的帳號/shuangquan-menu.git
cd shuangquan-menu

# 直接用瀏覽器開啟（需要本地伺服器以載入 JSON）
python3 -m http.server 8080
# 然後開啟 http://localhost:8080
```

---

*基隆市私立雙全幼兒園 餐點表系統 · 2025*
