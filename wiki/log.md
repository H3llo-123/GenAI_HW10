# Wiki Operation Log

## [2026-11-21] init | 專案結構與基礎檔案初始化

### 新增
- 建立 `wiki/` 目錄結構（`concepts/`, `reports/`, `comparisons/`, `examples/`）
- 建立 `wiki/index.md`：知識庫入口索引
- 建立 `wiki/log.md`：Wiki 操作紀錄
- 建立 `wiki/glossary.md`：專有名詞術語表
- 建立 `slides/` 目錄與初始 `slides/index.html`

### 說明
- 已研讀 `AGENTS.md` 規範。
- 完成專案基礎架構初始化，所有規範與限制（Single Source of Truth、Extend don't create、來源標註、需人工確認等）已就緒。
- 下一步準備依優先級處理 `01_會計學原理導論.pdf` 之 Ingest。

### 使用者確認
- 依使用者指示「先讀過AGENTS.md，並建立需要的資料夾及檔案」完成初始化。


## [2026-11-21] ingest | 01_會計學原理導論.pdf

### 新增頁面
- `wiki/concepts/accounting.md`：會計定義、商業語言、三項活動（辨認、記錄、溝通）與簿記之區別
- `wiki/concepts/accounting-users.md`：內部使用者（管理會計）與外部使用者（財務會計）
- `wiki/concepts/accounting-equation.md`：基本會計恆等式、獨資/合夥/公司等式改寫、進階展開式
- `wiki/concepts/assets.md`：資產三大要件（過去事件、控制、未來效益）與排除預期交易
- `wiki/concepts/liabilities.md`：負債三大要件（過去事件、現時義務、資源流出）與排除未來承諾
- `wiki/concepts/equity.md`：權益定義（剩餘權利、淨資產）、四大增減項目、股利本質與發放上限
- `wiki/concepts/transactions.md`：交易判定準則（改變財務狀況與否）與分析程序
- `wiki/concepts/accounting-assumptions.md`：企業個體假設與貨幣單位衡量假設
- `wiki/concepts/recognition-and-measurement.md`：認列兩大條件、歷史成本與公允價值三面向
- `wiki/reports/financial-statements-overview.md`：四大報表體系、編製勾稽順序、資訊品質特性
- `wiki/reports/balance-sheet.md`：資產負債表（財務狀況表）、特定時點存量資訊
- `wiki/reports/income-statement.md`：損益表、特定期間流量資訊、淨利計算與結轉
- `wiki/comparisons/bookkeeping-vs-accounting.md`：簿記與會計之層次、核心任務與產出比較
- `wiki/comparisons/balance-sheet-vs-income-statement.md`：時點vs期間、存量vs流量、財務狀況vs經營成果之對照
- `wiki/examples/beverage-shop.md`：清爽茶飲店第一階段 10 筆基本交易分析與恆等式平衡彙總表

### 更新
- `wiki/index.md`：收錄 15 篇新增頁面之索引連結與一句話摘要，將 01 移至已完成 Ingest
- `wiki/glossary.md`：新增 29 項會計專業名詞定義、英文對照與來源出處

### 發現問題與差異
- 原始教材在不同章節穿插使用「業主權益」與「股東權益」，已依專案規範統一以「權益 (Equity)」為主體，並於術語表中記錄組織脈絡差異。
- 借貸分錄（Debit / Credit）法則未出現於本篇，依教材進度保留至 `02_基本簿記.pdf` 處理。
- 現金流量表依規範僅於報表概論中以一句話帶過，不另立獨立頁面。

### 需人工核對
- `wiki/examples/beverage-shop.md`：改編自教材 Softbyte 公司 10 筆交易之情境與數字對照，標記為「需人工核對」。

### 使用者確認
- 使用者回覆「同意確認」，依審查通過之計畫執行寫入與索引更新。


## [2026-11-21] ingest | 02_基本簿記.pdf

### 新增頁面
- `wiki/concepts/debit-credit.md`：借貸法則本質（左與右）、T字帳結構、各要素借貸增減方向與正常餘額（Normal Balance）
- `wiki/concepts/double-entry.md`：複式簿記制度本質（有借必有貸，借貸必相等）、效益與記錄前置三程序
- `wiki/concepts/journal-and-entry.md`：普通日記簿（序時帳簿）、標準分錄格式、簡單分錄與複合分錄之借貸平衡
- `wiki/concepts/ledger-and-posting.md`：總分類帳、會計科目表結構化編碼（1資產~5費用）與過帳交互勾稽流程
- `wiki/reports/trial-balance.md`：試算表定義、編製三步驟、五大局限性與除以2（方向放反）、除以9（換位錯誤）之查錯法則
- `wiki/comparisons/journal-vs-ledger.md`：普通日記簿（交易全貌/時間順序/錄影帶）與總分類帳（科目分類/餘額歷史/檔案夾）之對照與互補

### 擴充既有頁面 (Extend)
- `wiki/concepts/accounting-equation.md`：擴充會計恆等式左右兩邊與借貸平衡之數學對應關係
- `wiki/concepts/transactions.md`：補充聘僱員工簽約未達交易標準之釋例，以及交易分析如何銜接分錄寫作
- `wiki/examples/beverage-shop.md`：擴充第二階段——將清爽茶飲店 10 筆交易完整轉換為借貸分錄（日記簿）、T 字帳過帳示意與試算表平衡驗證

### 更新
- `wiki/index.md`：新增 6 篇新頁面索引與摘要，更新既有頁面描述，將 02 移至已完成 Ingest
- `wiki/glossary.md`：新增 15 項核心術語（借方、貸方、正常餘額、複式簿記、日記簿、分錄、簡單分錄、複合分錄、分類帳、過帳、會計科目表、試算表、預收服務收入、預付保險費、換位錯誤）

### 發現問題與關鍵澄清
- 釐清借貸（Dr. / Cr.）純屬位置代號（左與右），與日常生活之借款貸款完全無關。
- 釐清「預收服務收入」實質為負債、「預付保險費」實質為資產之初學易混淆科目。
- 強調試算表借貸相等僅能保證數學平衡，無法保證無漏記、重記或科目誤用。

### 需人工核對
- `wiki/examples/beverage-shop.md`：手搖飲店第二階段 10 筆分錄之借貸方向、金額與 T 字帳結算餘額。

### 使用者確認
- 使用者回覆「同意確認」，依審查通過之計畫執行寫入、擴充與日誌更新。


## [2026-11-21] ingest | 03_調整分錄.pdf

### 新增頁面
- `wiki/concepts/adjusting-entries.md`：調整分錄定義、為什麼需要調整分錄（會計期間假設＋應計基礎＋配合原則 vs 未調整試算表之局限）、會計循環中串聯調整後試算表之角色、影響報表之兩大鐵律（絕不涉及現金、必同時跨損益與資產負債要素）、遞延與應計兩大類別提綱

### 擴充既有頁面 (Extend)
- `wiki/concepts/accounting-assumptions.md`：擴充「會計期間假設 (Time Period Assumption / Periodicity)」、會計年度 (Fiscal Year) 與曆年制 (Calendar Year)、期中期間劃分，以及人為切斷期間如何引發應計與調整需求
- `wiki/reports/financial-statements-overview.md`：補充「調整後試算表 (Adjusted Trial Balance)」為直接編製正式四大財務報表的前置依據與銜接關係

### 更新
- `wiki/index.md`：新增 `[[adjusting-entries]]` 條目，更新 `[[accounting-assumptions]]` 與 `[[financial-statements-overview]]` 摘要，將 03 移至已完成 Ingest
- `wiki/glossary.md`：新增 11 項核心術語（應計基礎、現金基礎、會計期間假設、會計年度、曆年制、調整分錄、配合原則、收入認列原則、遞延項目、應計項目、調整後試算表）

### 遵循規範與關鍵澄清
- 嚴格遵守 AGENTS.md 規範第 4.1、4.2、6.2 與 11 節輕量處理原則：深入聚焦於「為什麼需要調整」、「在會計循環中的角色」與「與財務報表的關係」，堅決不引入複雜的折舊計算、記實轉虛/記虛轉實之雙重記帳法，以及 IFRS 15 收入認列五步驟之細節分錄。
- 確立調整分錄兩大鐵律：**絕不涉及現金科目**，且**必定同時涉及損益表科目與資產負債表科目**。

### 需人工核對
- `wiki/concepts/adjusting-entries.md`：手搖飲店紙杯耗用（2,400 元）與工讀生應計薪資（5,000 元）為教學假設情境。

### 使用者確認
- 使用者回覆「確認」，依審查通過之輕量 Ingest 計畫執行寫入、擴充與日誌更新。


## [2026-11-21] ingest | 04_完整的會計循環.pdf

### 新增頁面
- `wiki/concepts/accounting-cycle.md`：會計循環 9 大步驟全貌與階段劃分、暫時性帳戶（虛帳戶）vs 永久性帳戶（實帳戶）本質對照、結帳分錄（結清歸零與損益彙總過渡科目）、結帳後試算表（驗證新期間起跑點平衡）、工作底稿非正式草稿定位、清爽茶飲店 12 月底完整循環結帳演練

### 擴充既有頁面 (Extend)
- `wiki/concepts/accounting-assumptions.md`：擴充第 4 項核心假設「繼續經營假設 (Going Concern Assumption)」、評估期間（至少12個月）、排除清算價值與維持歷史成本衡量之依據
- `wiki/reports/financial-statements-overview.md`：擴充整份財務報表要素與「同等重要性 (equal prominence)」及「交互索引」原則；完整深化觀念架構下主要使用者之一般目的需求、基本品質特性（攸關性、忠實表達、重大性）、強化品質特性（可比、可驗證、時效、可了解）與成本限制 (Cost Constraint)
- `wiki/reports/balance-sheet.md`：擴充分類資產負債表（流動與非流動項目）、營業週期 (Operating Cycle) 劃分標準（1 年或營業週期較長者）、流動負債比重對短期償債壓力之財務意涵、資產與負債內部排序結構

### 更新
- `wiki/index.md`：收錄 `[[accounting-cycle]]`，更新 assumptions、overview 與 balance sheet 摘要，將 04 移至已完成 Ingest
- `wiki/glossary.md`：新增 19 項核心術語（會計循環、結帳分錄、暫時性帳戶/虛帳戶、永久性帳戶/實帳戶、損益彙總、結帳後試算表、工作底稿、流動資產、非流動資產、流動負債、非流動負債、營運週期、繼續經營假設、重大性、可比性、可驗證性、時效性、可了解性、成本限制）

### 遵循規範與關鍵澄清
- 嚴格遵守 AGENTS.md 規範第 4.1 與 4.2 節中等優先級原則：以梳理「會計處理流程」與「報表產出關係」為核心，不要求初學者掌握完整繁複的會計操作；排除改正分錄之跨期保留盈餘追溯調整、選擇性迴轉分錄之借貸對調技術、十欄式工作底稿之繁複演算，以及債務違約重協議之判定。
- 深刻貫通學習成果 3：透過虛帳戶（期末歸零）與實帳戶（餘額結轉下期）的記帳制度，透徹解釋損益表「期間流量」與資產負債表「時點存量」的底層會計機制。

### 需人工核對
- `wiki/concepts/accounting-cycle.md`：清爽茶飲店 12 月底服務收入 25,000 元、費用 17,000 元、淨利 8,000 元與股利 2,000 元之結帳分錄數字為「教學假設」。

### 使用者確認
- 使用者回覆「確認」，依審查通過之計畫執行寫入、擴充與日誌更新。


## [2026-11-21] ingest | 05_買賣業會計.pdf

### 新增頁面
- `wiki/concepts/merchandising-accounting.md`：買賣業會計基礎、買賣業相較於服務業的三大核心差異（商品型態、存貨資產、營業週期拉長）、多出之關鍵科目（商品存貨、銷貨成本、銷貨毛利、毛利率）、買賣商品之雙重認列機制、成本流動公式（可供銷貨成本劃分）、永續盤存制 vs 定期盤存制概念對比、FOB 交貨條件（起運點 vs 目的地）與進銷折讓常識

### 擴充既有頁面 (Extend)
- `wiki/reports/income-statement.md`：擴充買賣業「多步驟損益表 (Multiple-Step Income Statement)」四層分級架構（銷貨淨額 $\rightarrow$ 銷貨毛利 $\rightarrow$ 營業淨利 $\rightarrow$ 本期淨利），以及銷貨毛利率對商品定價與獲利能力之財務分析意義
- `wiki/examples/beverage-shop.md`：依 AGENTS.md 第 7.1 節規範，擴充「第三階段：延伸至買賣業」——清爽茶飲店兼售「品牌保溫杯」，演示批發購入 100 個保溫杯（存貨 15,000 元）、零售賣出 60 個保溫杯（收現 15,000 元、結轉銷貨成本 9,000 元、實現銷貨毛利 6,000 元）之雙重分錄與恆等式平衡

### 更新
- `wiki/index.md`：收錄 `[[merchandising-accounting]]`，更新 `[[income-statement]]` 與 `[[beverage-shop]]` 摘要，將 05 移至已完成 Ingest，標記全數五份原始教材 Ingest 圓滿達成
- `wiki/glossary.md`：新增 15 項核心術語（買賣業、商品存貨、銷貨收入、銷貨成本、銷貨毛利、銷售毛利率、銷貨淨額、銷貨退回與讓價、銷貨折扣、可供銷貨成本、起運點交貨、目的地交貨、永續盤存制、定期盤存制、多步驟損益表）

### 遵循規範與關鍵澄清
- 嚴格遵守 AGENTS.md 規範第 4.1、4.2 與 6.3 節輕量處理原則：聚焦回答買賣業與服務業差異、多出項目與買賣商品對會計之影響三大問題，排除定期盤存制進銷結帳細節分錄、進銷折讓年化利率計算、工作底稿演算與附錄 5C 估計退款負債等超出初學範圍之細節。
- 貫穿案例保持高度一致性：維持「清爽茶飲店」與「張老闆」主體，所有買賣業交易數字與恆等式嚴謹平衡，並標註為教學假設。

### 需人工核對
- `wiki/examples/beverage-shop.md`：第三階段保溫杯進銷數字（批發價 150、售價 250、毛利 6,000）為「教學假設」。

### 使用者確認
- 使用者回覆「確認」，依審查通過之輕量 Ingest 計畫執行寫入、擴充與日誌更新。


## [2026-11-21] slides | 最終 HTML 教學簡報產出

### 產出檔案
- `slides/index.html`：共 18 頁響應式互動教學簡報，嚴格以 `wiki/` 知識庫為唯一知識來源（Single Source of Truth），無任何外部模型知識補遺。

### 涵蓋階段與主題架構
1. **Slide 1**：封面與四大學習成果導覽（[[index]]）
2. **Slide 2**：第一講：會計是什麼？商業通用語言（辨認 $\rightarrow$ 記錄 $\rightarrow$ 溝通，簿記 vs 會計）（[[accounting]], [[bookkeeping-vs-accounting]]）
3. **Slide 3**：第二講：誰會使用會計資訊？內部使用者（管理會計）vs 外部使用者（財務會計）（[[accounting-users]]）
4. **Slide 4**：第三講：會計三大要素（資產、負債、權益之定義與要件）（[[assets]], [[liabilities]], [[equity]]）
5. **Slide 5**：第四講：會計基石——會計恆等式（資產＝負債＋權益，權益四大驅動力）（[[accounting-equation]], [[equity]]）
6. **Slide 6**：恆等式實戰：清爽茶飲店開張前三筆交易之天平平衡（[[beverage-shop]]）
7. **Slide 7**：延伸思考：什麼才算會計上的「交易」？面試簽約 vs 發薪水（[[transactions]]）
8. **Slide 8**：第五講：借貸法則本質（借左貸右，T字帳增減方向與正常餘額）（[[debit-credit]]）
9. **Slide 9**：複式簿記：有借必有貸，借貸必相等（帕喬利智慧與前置三程序）（[[double-entry]], [[journal-and-entry]]）
10. **Slide 10**：第六講：手把手寫出第一筆借貸分錄（簡單分錄 vs 複合分錄實例）（[[journal-and-entry]], [[beverage-shop]]）
11. **Slide 11**：過帳與試算表：檢查天平平衡（日記簿錄影帶 vs 分類帳檔案夾，除以2與除以9查錯法）（[[ledger-and-posting]], [[trial-balance]], [[journal-vs-ledger]]）
12. **Slide 12**：第七講：兩大財務報表對決（資產負債表存量快照 vs 損益表期間流量，勾稽關係）（[[balance-sheet-vs-income-statement]], [[balance-sheet]], [[income-statement]]）
13. **Slide 13**：讀懂資產負債表：流動與非流動之秘密（營業週期標準、流動負債償債壓力）（[[balance-sheet]], [[assets]], [[liabilities]]）
14. **Slide 14**：讀懂損益表：多步驟分層的獲利密碼（毛利、毛利率、營業利益、本期淨利）（[[income-statement]], [[merchandising-accounting]]）
15. **Slide 15**：第八講：會計循環與期末結清（9 大步驟、調整分錄鐵律、虛帳戶歸零 vs 實帳戶結轉）（[[accounting-cycle]], [[adjusting-entries]]）
16. **Slide 16**：延伸應用：手搖飲店兼售保溫杯（買賣業雙重認列、成本流動公式）（[[merchandising-accounting]], [[beverage-shop]]）
17. **Slide 17**：報表背後的隱形支柱：四大會計假設（企業個體、貨幣單位、會計期間、繼續經營）（[[accounting-assumptions]]）
18. **Slide 18**：第九講：學習成果大驗收（互動點擊自測四項核心能力）（[[index]]）

### 規範驗收確認
- [x] 18 頁投影片完全符合 15～20 頁之規格要求。
- [x] 所有內容與案例數字皆可在 Wiki 中追溯，原始碼皆具備 `Wiki Sources` 標註。
- [x] 完整覆蓋四項核心學習成果，並以清爽茶飲店（張老闆）貫穿全篇。
- [x] 具備互動導覽（鍵盤左右鍵、空白鍵、點擊按鈕、進度條、點擊揭示解答）。
