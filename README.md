# 文件治理起手式(KMU 學生學習範例)

> A minimal document-governance starter kit for KMU students, by eros_tsung_pao_lin.
> 授權:CC BY 4.0(可自由改作,標示來源即可)

## 這是什麼

這是一個「用 git + Claude Code 管理文件」的最小治理架構範本,
給高雄醫學大學的學生作為起點,用來管理:

- **社團文件**(會議紀錄、活動企劃、交接資料)
- **大專生研究計畫**(申請書、進度紀錄、數據與報告)
- **自學筆記**(課程筆記、讀書心得、技能學習)

它刻意做得很小:只有一套常駐規範(`CLAUDE.md`)、一本決策紀錄、
三個用途目錄。**骨架給你,血肉自己長**——怎麼長,見
[治理擴增指南](治理擴增指南.md)。

## 快速開始

1. **建立你自己的 repo,並設為 private**——你的社團文件與研究計畫內容不適合公開。兩種做法擇一:
   - 在 GitHub 網頁按右上角綠色的「Use this template」
     (不建議用 Fork:公開 repo 的 fork 會被強制維持公開,無法轉 private。)
     建好後把它抓到自己電腦:建議用 [GitHub Desktop](https://desktop.github.com/),
     登入 GitHub 後選 File → Clone repository,選剛建的 repo。
     熟悉終端機的人也可用 `git clone <你的 repo 網址>`,
     但 private repo 要先登入 GitHub(例如執行 `gh auth login`),
     否則會要求帳密而失敗。
     之後在終端機用 `cd` 進入該資料夾,打 `claude` 啟動 Claude Code
     (桌面版則在新對話選擇該資料夾)。
   - 用 Claude Code 安裝 [doc-governance](https://github.com/SynchronicEros/claude-code-doc-governance-zh),
     在本機資料夾對 Claude 說「建立治理架構」。用這個方式的人本步已完成;
     要放上 GitHub 時再建 private repo。
2. 讀完 [CLAUDE.md](CLAUDE.md)——這是整個架構的核心,
   Claude Code 在這個 repo 工作時會自動遵守它。
3. 把你的文件放進對應目錄,各目錄的 `README.md` 有該用途的治理要點。
4. 遇到重要決定,記進 [決策紀錄.md](決策紀錄.md)。
5. 架構不夠用了,照 [治理擴增指南](治理擴增指南.md) 升級。

### 只用 Codex(不用 Claude Code)的人

1. 用快速開始第 1 步的第一種做法(Use this template 加 GitHub Desktop)
   建 repo 並抓到電腦,在該資料夾開 Codex。
2. 對 Codex 說:
   「請在這個資料夾建立 AGENTS.md,內容只寫一行:
   本 repo 的規範見 CLAUDE.md,開工前先讀並遵守。」
3. 規範只維護 `CLAUDE.md` 一份;裡面寫「Claude Code」之處,
   對 Codex 一樣適用。快速開始第 2–5 步照常進行。

## 更新紀錄

- 2026-10-09:「只用 Codex 的人」獨立成一節;clone 建議新手用 GitHub Desktop。
- 2026-10-09:快速開始補「用 doc-governance 在本機建立」與「只用 Codex 的人加 AGENTS.md」兩種做法。同日再補:用 Use this template 建立後如何抓到電腦並在資料夾啟動 Claude Code;Codex 使用者同走此路,CLAUDE.md 對 Codex 一樣適用。
- 2026-10-05:CLAUDE.md〈三、刪除規則〉新增一條:`LICENSE` 與 README〈授權與致謝〉不得刪除或修改(README 其他內容可改寫)。已用本範本建立 repo 的人,需要的話對照自行加入。
- 2026-10-04:[治理擴增指南](治理擴增指南.md)新增「隨時可加:兩條小規則」(刪除前判斷原始檔、決策紀錄登錄門檻),階段一補「引用文獻回原文核對」。已用本範本建立 repo 的人,範本更新不會自動同步到你的 repo,需要的話對照自行加入。

## 目錄結構

| 路徑 | 內容 |
|------|------|
| `CLAUDE.md` | 常駐規範:語言、版本規則、刪除規則、工作紀律、資料層級 |
| `決策紀錄.md` | 歷次重要決定的代號、選項與理由 |
| `治理擴增指南.md` | 從極簡架構長出完整治理的路線圖 |
| `社團文件/` | 社團營運文件,治理要點見目錄內 README |
| `研究計畫/` | 大專生研究計畫文件,治理要點見目錄內 README |
| `自學筆記/` | 個人學習紀錄,治理要點見目錄內 README |

## 核心理念(三句話)

1. **規範寫下來,不放在腦裡**——你會忘,組員會換,AI 讀得到檔案讀不到默契。
2. **每件事實只有一個正本**——同一資訊存兩處,遲早其中一處是錯的。
3. **先裁定,後動工**——重要修改先列選項與利弊,決定了才動手,並留下紀錄。

## 授權與致謝

- 本範本以 [CC BY 4.0](LICENSE) 授權釋出,作者 eros_tsung_pao_lin(KMU)。
- 改作時請保留來源標示;你自己放進 repo 的文件內容,授權由你自定
  (建議在你的 README 註明)。
