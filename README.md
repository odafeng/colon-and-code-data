# Colon & Code — 教材資料下載

這是 YouTube 頻道 **Colon & Code | 黃士峯 Fredric Huang** 的「**實戰專案 Build-Along**」系列的配套資料。
跟著影片一起做的話,把對應集數的資料下載下來即可。

> ⚠️ **所有資料皆為「虛構合成」**:姓名、病歷號、生日、檢驗值、結果……全部都是程式假造的,**與任何真實病人或研究無關**,僅供教學練習使用,不構成任何臨床建議。

## 怎麼下載
- **整包 clone**(順便練 Git):
  ```bash
  git clone https://github.com/odafeng/colon-and-code-data.git
  ```
- **只抓單一檔案**:在 GitHub 上點進該檔 → 右上角「Download raw file」。

---

## EP1 ｜拿到資料,先別分析、先「診斷」它
檔案:[`EP1_cohort/cohort_extract.xlsx`](EP1_cohort/cohort_extract.xlsx)
情境:一份「內科住院病人 30 天再入院」的資料中心萃取檔(48 列 × 17 欄),**故意做得很「髒」**,給你練習診斷:

| 欄位 | 說明 |
|---|---|
| 姓名 / 病歷號 / 生日 | ⚠️ **可識別個資**(教你第一步要挑出來去識別化;生日還故意混了三種日期格式) |
| 性別 / 年齡 | 人口學 |
| 入院日期 / 出院日期 / 住院天數 | 時間與住院長度 |
| 主診斷 / 糖尿病 / 高血壓 | 診斷與共病 |
| WBC / Hb / Cr | 檢驗值(故意有少量缺漏) |
| 出院衛教介入 | 暴露(exposure):有沒有做出院衛教 |
| 出院前用藥衛教 | ⚠️ **故意幾乎全空**——示範「關鍵 factor 根本沒收到」 |
| 再入院_30天 | 結果(outcome):30 天內有沒有再入院 |

📺 影片:https://youtu.be/QYgfWLpRLFc

---
資料以 [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) 釋出(本來就是假資料,隨意取用)。
