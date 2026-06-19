# Unit09半導體產業與股市分析 (Semiconductor & Stock Analysis)

## Environment Setup (環境建置)
<img width="1390" height="860" alt="image" src="https://github.com/user-attachments/assets/5050e338-5c53-49ea-98d9-c2360bfa34ee" />

# Phase 1: 單一公司深度分析 (TSMC Case Study)
### Lab 20-01: Fetch Data 題目: 下載台積電 (2330.TW) 近 5 年的股價資料。 目的: 獲取 raw data。
<img width="797" height="394" alt="image" src="https://github.com/user-attachments/assets/30fbd491-d42f-4757-aaf2-47965b6be697" />

## Chart 01: 收盤價走勢 (Close Price)
###  題目: 畫出每日收盤價 (Close) 的折線圖。 Insight: 觀察股價的長期趨勢 (Trend).
<img width="737" height="395" alt="image" src="https://github.com/user-attachments/assets/3ea12141-475e-4a20-a33a-bbc1f9b35bb4" />

## Chart 02: 交易量 (Volume)
###  題目: 畫出每日交易量的長條圖。Insight: 爆量通常意味著大事件發生 (財報公佈、地緣政治)。
<img width="1126" height="508" alt="image" src="https://github.com/user-attachments/assets/4cdd3ccb-e3b9-4966-b9e5-e42fffc6ca1b" />

## Chart 03: 均線策略 (SMA Golden Cross)
###  題目: 計算並畫出 SMA 60 (季線) 與 SMA 20 (月線)。Insight: 黃金交叉 (短線穿過長線) 視為買入訊號？
<img width="1115" height="775" alt="image" src="https://github.com/user-attachments/assets/86fe14e9-937b-4d42-af87-179702eaa5ef" />

##  Chart 04: 日收益率 (Daily Return)
###  題目: 計算每日變動百分比 pct_change()。Insight: 股價是有雜訊的，Return 呈現平均為 0 的波動。
<img width="1139" height="521" alt="image" src="https://github.com/user-attachments/assets/f4474ef2-29e1-4162-859f-70627620d27b" />

## Chart 05: 收益率分佈 (Histogram)
### 題目: 畫出收益率的直方圖。Insight: 呈現常態分佈 (Normal Distribution) 或是肥尾 (Fat Tail)？
<img width="833" height="576" alt="image" src="https://github.com/user-attachments/assets/8452f5ab-e4ec-4a30-9b32-77efd656fb06" />

## Chart 06: 收益率箱型圖 (Return Boxplot)
###  題目: 找出極端值 (Outliers)。Insight: 那些圓點代表當日大漲或大跌的日子。
<img width="794" height="574" alt="image" src="https://github.com/user-attachments/assets/aea07445-2b57-4c82-a129-7934eca8702a" />

## Chart 07: 累積報酬率 (Cumulative Return)
### 題目: 假設第一天投入 1 元，現在變多少？ (1 + r).cumprod().Insight: 複利的力量。
<img width="1078" height="706" alt="image" src="https://github.com/user-attachments/assets/6d1075f0-1ba6-4923-802b-49997532ece6" />

## Chart 08: 產業市佔 (Market Share Pie)
### 題目: 手動建立 Foundry 市佔資料並繪製圓餅圖。Insight: 視覺化 TSMC 的統治地位。
<img width="977" height="562" alt="image" src="https://github.com/user-attachments/assets/68215f9f-ccc4-448c-8577-6511c8b24299" />

## Phase 2: 競品大亂鬥 (Industry Comparison)
### Lab 20-02: Multi-Stock Data
#### 題目: 下載 TSM, NVDA, INTC, AMD 四家公司資料。目的: 建立比較基準
<img width="949" height="289" alt="image" src="https://github.com/user-attachments/assets/13c1797b-9f80-4ff0-8973-33c2990cb62a" />

##  Chart 09: 收盤價比較 (Raw Price)
### 題目: 直接畫出四家公司股價。Insight: 那支股價太高壓扁其他人，無法比較趨勢。
<img width="1216" height="651" alt="image" src="https://github.com/user-attachments/assets/2c5c2c72-034a-4a91-85af-88a8ed8cd29b" />

## Chart 10: 正規化比較 (Normalized Base 100)
### 題目: 將所有股價除以第一天股價 * 100。Insight: 清楚看到誰成長最快。
<img width="1175" height="658" alt="image" src="https://github.com/user-attachments/assets/666ddeaa-eb98-44ff-a884-7017123df791" />

## Chart 11: 相關性熱圖 (Correlation Heatmap)
### 題目: 計算收益率的相關係數。Insight: TSM 與 NVDA 相關性高嗎？INTC 是否脫鉤？
<img width="742" height="637" alt="image" src="https://github.com/user-attachments/assets/8e032501-6ba6-4dfc-8872-f0e4d5a8abb5" />

## Chart 12: 散佈圖比較 (Scatter: NVDA vs TSM)
### 題目: 觀察兩家公司收益率的線性關係。Insight: 正相關意味著連動性高。
<img width="774" height="586" alt="image" src="https://github.com/user-attachments/assets/40e81abd-201c-45f5-8452-b6e71e64936c" />

## Chart 13: 散佈圖矩陣 (PairGrid)
### 題目: 一次看清所有公司的兩兩關係。
<img width="1147" height="1069" alt="image" src="https://github.com/user-attachments/assets/f98dd8e6-9727-4e0f-aeac-93f528307f72" />

## Chart 14: 風險分析 (Risk Bar)
### 題目: 比較各公司的年化波動率 (Std * sqrt(252)).Insight: NVDA 成長高但波動也大，TSM 相對穩健?
<img width="1093" height="629" alt="image" src="https://github.com/user-attachments/assets/037f5646-dc24-47f4-9504-cb1ca16b92cb" />

## Chart 15: 總報酬分析 (Return Bar)
### 題目: 期間總報酬率比較。
<img width="781" height="604" alt="image" src="https://github.com/user-attachments/assets/8869dc1d-8e58-4ad0-a8d8-57bc51286681" />

# Phase 3: 進階視覺化 (Advanced Techniques)
## Chart 16: 滾動波動率 (Rolling Volatility)
### 題目: 觀察 TSM 波動率隨時間的變化 rolling(30).std()。Insight: 找出市場最恐慌的時期。
<img width="1243" height="523" alt="image" src="https://github.com/user-attachments/assets/0ab5cde6-2e3d-4e28-a7f1-7a01fa6df9f6" />

##  Chart 17: 回撤分析 (Drawdown Area)
### 題目: 計算從歷史高點跌了多少 (price / running_max) - 1。Insight: 水下圖 (Underwater Plot)，評估最大虧損風險。
<img width="1136" height="533" alt="image" src="https://github.com/user-attachments/assets/48a2dbed-ce49-45df-82a8-5da29a83e949" />

## Chart 18: K線圖 (Candlestick - Basic)
### 題目: 繪製最後 60 天的 K 線圖 (使用 mplfinance 或手刻)。
<img width="917" height="635" alt="image" src="https://github.com/user-attachments/assets/3e99c879-74c6-4a7f-bc08-6d1ad026a54b" />

## Chart 19: 布林通道 (Bollinger Bands)
### 題目: MA20 +/- 2倍標準差。Insight: 超跌與超買訊號。
<img width="1248" height="839" alt="image" src="https://github.com/user-attachments/assets/7a79bcab-6256-4cf6-80cd-ead6fb2e0486" />

## Chart 20: 每日漲跌幅分佈 (Violin Plot)
### 題目: 使用小提琴圖檢視每年或每月的收益分佈。Insight: 結合 Boxplot 與 Histogram 的特性。
<img width="811" height="599" alt="image" src="https://github.com/user-attachments/assets/344c3b54-1594-4a54-898a-7c914d3a02cb" />



