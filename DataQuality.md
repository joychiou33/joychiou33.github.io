
## 數據質量管理流程工作流程
![image](https://user-images.githubusercontent.com/117702322/216874076-7f282a19-5478-4c76-8987-764886ee464e.png)
[2022 數據質量管理辦法](https://blog.csdn.net/weixin_43597208/article/details/125287467?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167564887416782427499517%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=167564887416782427499517&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~baidu_landing_v2~default-3-125287467-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B0%E6%8D%AE%E8%B4%A8%E9%87%8F%E7%AE%A1%E7%90%86&spm=1018.2226.3001.4449)  

在數據質量監控過程中產生的告警信息，數據質量管理實施部門應在規定的時限內開展告警信息分析，並對告警產生的原因作出判定。對於**一般性告警信息**即系統運行環境異常或操作失誤等導致的、具有偶發性、在短期內恢復且不產生嚴重後果的數據質量監控告警。數據質量管理實施部門可直接按照操作規程給予處理，如：系統斷電等原因產生的告警；對於嚴重告警信息，應將告警產生的問題通告技術主管部門和相關業務部門。技術承辦單位應協助數據質量管理實施部門解決問題的工作。對已處理的數據質量問題，數據質量管理實施部門應將問題處理結果在規定時限內通告技術主管部門、業務主管部門和技術承辦單位。各相關部門收到數據質量問題處理結果後確認結果和建議反饋。數據質量管理實施部門應定期編寫數據質量監控報告，歸檔備查。

- 數據質量監控 data quality control  
獲取業務各環節的數據質量信息，結合有關檢查規則和採集規則，對數據質量情況進行診斷，並及時向數據質量管理實施部門報告的活動。根據告警所反映的數據質量現象的嚴重程度、影響範圍，設定嚴重性程度不同的告警級別。每一級別告警信息的發送都應具備多種送達手段。從數據採集、預警分析到告警生成，每個階段都需進行程序化管理。
- 數據質量評估 data quality assessment  
由數據質量管理實施部門根據需要發起，得到評估結果並作為依據評估指標和評估方法進行評價，數據質量改進的參考和依據。
- 數據質量報告 data quality report  
對數據質量日常監控以及質量評估等過程累積的各種信息進行匯總、梳理、統計和分析，形成統計報告的過程。數據質量報告的發布具有一定的時效性。用戶應在所賦權限範圍內查看質量報告，防止信息洩露。數據質量報告的歸檔要求將相關報告按照分類,作為後續數據質量問題處理和分析的參照。
- 數據質量知識 data quality knowledge  
在數據質量管理活動中獲取的有關數據質量問題處理的經驗和成果。數據質量知識主要來源於對數據質量問題的記錄與總結，以及對問題解決過程自身的知識評價。數據質量知識的產生與利用過程是一個互相促進改良的過程，為數據質量管理的其他活動提供重要的支撐。



## 設立數據安檢站
![image](https://user-images.githubusercontent.com/117702322/216894950-25a6605b-3ac4-4c46-a1be-26fcb18d0ba3.png)
[2020 如何保障數據準確性](https://zhuanlan.zhihu.com/p/98277328)  
[2022 引擎數據質量解決方案和最佳實踐](https://blog.csdn.net/WindyQCF/article/details/123725748?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565602116800217045802%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565602116800217045802&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-27-123725748-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449)  
## 數據質量保障原則
- 完整性 Completeness
數據是完整不缺失的。例如人員信息完整涵蓋性別、年齡等。
- 及時性
數據在時間變化中的正確程度，數據更新、修改和提取等的快速性程度。例如是否有時間戳記。
- 一致性
同源或跨源的數據是一致不衝突的。例如同一個人在不同源取過來的性別都是一致的。
- 唯一性 Uniqueness
數據是唯一不重複的，主要包括PK和FK。例如同一個ID沒有重複記錄。
- 規範性 Conformity
數據是規範統一的，數據格式、類型、域值和業務規則的有效性，數據的關聯是不缺失的。例如時間信息都以yyyy-mm-dd格式存儲、兩張表建立的關聯關係存在，不丟失數據。
- 準確性 Accuracy
數據是準確合理的，如計量誤差、度量單位等方面。例如年齡在合理範圍內。  
※偏移量、非空檢查、值域檢查、規範性檢查、重複性檢查、關聯關係檢查、離群值檢查、波動檢查等等  

|維度|分類|
|--|--|
|完整性/及時性|是否有數據(空白/0/筆數檢查)|
|一致性/唯一性/規範性|檢查重複(PK)/關聯(FK)/格式(正規表示式)|
|準確性|值域、離群值、波動檢查|

[*2022 数据质量(DQ)](https://blog.csdn.net/hsabrina/article/details/124860003?ops_request_misc=&request_id=&biz_id=102&utm_term=%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-1-124860003.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&spm=1018.2226.3001.4449)  
[2020 數據審核](https://blog.csdn.net/huryer/article/details/104433547)  
[2020 數據修正](https://blog.csdn.net/huryer/article/details/104434312)  
[2020 數據質量管理_第一篇檢查指標](https://blog.csdn.net/ab19920904/article/details/106399538?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565602116800217045802%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565602116800217045802&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-17-106399538-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449)  
[TBIC 什麼是資料品質](https://www.tibco.com/zh-hant/reference-center/what-is-data-quality)  

[數據檢測程式碼實作][1](https://blog.csdn.net/weixin_44586883/article/details/120555303?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565602116800217045802%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565602116800217045802&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-14-120555303-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449) 
[2](https://blog.csdn.net/Ft_xPz/article/details/83343530?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565602116800217045802%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565602116800217045802&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-19-83343530-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449) 

## 影響數據質量的因素
主要就技術、業務、管理三個方面: 
- 技術  
數據模型設計的質量問題，例如：數據庫表結構、數據庫約束條件、數據校驗規則的設計開發不合理，造成數據錄入無法校驗或校驗不當，引起數據重複、不完整、不准確。  
數據源存在數據質量問題，例如：有些數據是從生產系統採集過來的，在生產系統中這些數據就存在重複、不完整、不准確等問題，而採集過程有沒有對這些問題做清洗處理，這種情況也比較常見。  
數據採集過程質量問題， 例如：採集點、採集頻率、採集內容、映射關係等採集參數和流程設置的不正確，數據採集接口效率低，導致的數據採集失敗、數據丟失、數據映射和轉換失敗。  
數據傳輸過程的問題，例如：數據接口本身存在問題、數據接口參數配置錯誤、網絡不可靠等都會造成數據傳輸過程中的發生數據質量問題。  
數據裝載過程的問題，例如：數據清洗規則、數據轉換規則、數據裝載規則配置有問題。  
數據存儲的質量問題，例如：數據存儲設計不合理，數據的存儲能力有限，人為後台調整數據，引起的數據丟失、數據無效、數據失真、記錄重複。  
業務系統各自為政，煙囪式建設，系統之間的數據不一致問題嚴重。  
- 業務  
業務需求不清晰，例如：數據的業務描述、業務規則不清晰，導致技術無法構建出合理、正確的數據模型。  
業務需求的變更，這個問題其實是對數據質量影響非常大的，需求一變，數據模型設計、數據錄入、數據採集、數據傳輸、數據裝載、數據存儲等環節都會受到影響，稍有不慎就會導致數據質量問題的發生。  
業務端數據輸入不規範，常見的數據錄入問題，如：大小寫、全半角、特殊字符等一不小心就會錄錯。人工錄入的數據質量與錄數據的業務人員密切相關，錄數據的人工作嚴謹、認真，數據質量就相對較好，反之就較差。  
數據作假，對，你沒看錯，就是數據作假！操作人員為了提高或降低考核指標，對一些數據進行處理，使得數據真實性無法保證。  
- 管理  
認知問題。企業管理缺乏數據思維，沒有認識到數據質量的重要性，重系統而輕數據，認為系統是萬能的，數據質量差些也沒關係。  
沒有明確數據歸口管理部門或崗位，缺乏數據認責機制，出現數據質量問題找不到負責人。  
缺乏數據規劃，沒有明確的數據質量目標，沒有製定數據質量相關的政策和製度。  
數據輸入規範不統一，不同的業務部門、不同的時間、甚至在處理相同業務的時候，由於數據輸入規範不同，造成數據衝突或矛盾。  
缺乏有效的數據質量問題處理機制，數據質量問題從發現、指派、處理、優化沒有一個統一的流程和製度支撐，數據質量問題無法閉環。  
缺乏有效的數據管控機制，對歷史數據質量檢查、新增數據質量校驗沒有明確和有效的控制措施，出現數據質量問題無法考核。  
### 數據自身的質量 和 數據的過程質量
數據自身的質量很好理解，比如數據必須真實準確地反映實際發生的業務，任何業務操作的數據都沒有被遺漏，數據存在各種約束條件，這種約束條件不能自相矛盾等等。  
數據的過程質量就是數據的使用過程符合標準規範，比如數據存儲：數據是否被安全地存儲到了合適的介質上，能夠保證數據不受外來因素的破壞。當然數據存儲只是數據使用過程的一個環節，除此之外還包括獲取、傳輸、應用和刪除等一系列的使用過程，這其實也是數據生命週期的各個階段。  

### 依據ISO9001 應用在數據治理方面
[2019 數據治理系列5：淺談數據質量管理](https://blog.csdn.net/kuangfeng88588/article/details/99085074?ops_request_misc=&request_id=&biz_id=102&utm_term=%E6%95%B0%E6%8D%AE%E8%B4%A8%E9%87%8F%E7%AE%A1%E7%90%86&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-2-99085074.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&spm=1018.2226.3001.4449)    

## 常見的數據監控原則
單表數據量監控
一張表的記錄數在一個已知的範圍內，或者上下浮動不會超過某個閾值

單表空值檢測
某個字段為空的記錄數在一個範圍內，或者佔總量的百分比在某個閾值範圍內

單表重複值檢測
一個或多個字段是否滿足某些規則

單表值域檢測
一個或多個字段沒有重複記錄

跨表數據量對比
主要針對同步流程，監控兩張表的數據量是否一致

數據質量的準則，監控方向大致有：
- 規範類：如表結構、表命名、字段命名、表註釋、文件路徑
- 業務類：責任人、歸屬的業務、血緣關係、分母是否為0、NUll值是否參與計算等
- 性能類：數據波動情況(增量數據行數、表全量總行數)、計算運行時長、資源消耗情況、大表提醒、重複計算監測、大小表join操作等

## 校驗規則
關聯性檢查: 兩個數據表的key值關聯是否存在。
行級別: 兩個數據表的數據量是否一致。
列級別: 兩個數據表的表結構是否一致，如字段數量、字段類型和寬度等是否一致。
內容級別: 兩個數據表的內容是否一致。其一數據表的內容是否缺失。
※ 應該可以用通用的**規則引擎**進行解決 
[2019 數據質量分析之校驗規則模板](https://blog.csdn.net/weixin_42893650/article/details/88743432)  

![image](https://user-images.githubusercontent.com/117702322/216877324-db32dc75-1362-4a09-9b81-7255a245d79c.png)
[2019 數據質量管理學習筆記](https://blog.csdn.net/weixin_42893650/article/details/88414509?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565242216800182777087%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565242216800182777087&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-1-88414509-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B0%E6%8D%AE%E8%B4%A8%E9%87%8F%E7%AE%A1%E7%90%86&spm=1018.2226.3001.4449)  
[2021 淺談數據質量管理](https://blog.csdn.net/ytp552200ytp/article/details/117290007?ops_request_misc=&request_id=&biz_id=102&utm_term=%E6%95%B0%E6%8D%AE%E8%B4%A8%E9%87%8F%E7%AE%A1%E7%90%86&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-6-117290007.nonecase&spm=1018.2226.3001.4449)  
[2021 數據質量管理：6個維度，50個檢查項](https://blog.csdn.net/mm_ren/article/details/119307351?ops_request_misc=&request_id=&biz_id=102&utm_term=%E6%95%B0%E6%8D%AE%E8%B4%A8%E9%87%8F%E7%AE%A1%E7%90%86&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-3-119307351.nonecase&spm=1018.2226.3001.4449)  


[2022 數據校驗規則](https://blog.csdn.net/qq_42217906/article/details/122882296?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565484916782427494545%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565484916782427494545&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-16-122882296-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449)  

[2022 數據清洗規範](https://blog.csdn.net/Cecilia_l/article/details/122714234?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565484916782427494545%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565484916782427494545&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-20-122714234-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449)  
[2022 數據標準--實戰](https://blog.csdn.net/ytp552200ytp/article/details/124793994#comments_25005020)


## 資料品質監控平台
Amazon建立了Deequ工具，Uber 則在部落格分享內部的 UDQ(Uber Data Quality Platform)是如何運作的，其餘工具Apache Griffin等，這可以協助我們了解常見的資料品質指標。
DQC 數據監控規則有強規則和弱規則：  
- 強規則：一旦觸發報警就會阻斷任務的執行（將任務置為失敗狀態，使下游任務不會被觸發執行）。
- 弱規則：只報警但不阻斷任務的執行。  

哪些數據需要配置DQC 規則、應該配置什麼規則，也需要根據數據資產等級來確定。例如A1、A2 類數據監控率要達到90% 以上，規則類型需要3 種以上，而不重要的數據資產沒有強制要求。  
- 監控範圍：上游所有任務
- 監控的異常：任務出錯、任務變慢、預警業務延遲
- 告警對象
- 何時告警：實時任務一般一小時校驗一次，離線任務一般在數據執行完馬上校驗
- 告警方式：短信、電話、飛書消息、郵件等

[2021 監控資料品質的旅程](https://www.minglunwu.com/notes/2021/data_quality.html)  
數據質量監控平台的核心部分，包括數據質量檢查規則的定義、數據質量檢查規則腳本、檢查規則執行引擎、數據質量檢查規則執行情況監控等。  
[2020 數據倉庫之數據質量監控](https://blog.csdn.net/Li_Jian_Hui_/article/details/108151311?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565601916800180627932%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565601916800180627932&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-23-108151311-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449)  
[2019 利用數據質量規則庫推動數據質量管理](https://blog.csdn.net/wsdc0521/article/details/102838783?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565484916782427494545%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565484916782427494545&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-6-102838783-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449)  
[2021 基於DolphinScheduler 的數據質量檢查實踐](https://blog.csdn.net/DolphinScheduler/article/details/119951778?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565601916800180627932%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565601916800180627932&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-14-119951778-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449)  
[2022 數據質量流程與工具](https://dataclub.blog.csdn.net/article/details/122613169?spm=1001.2101.3001.6650.8&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ERate-8-122613169-blog-122919242.pc_relevant_3mothn_strategy_and_data_recovery&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ERate-8-122613169-blog-122919242.pc_relevant_3mothn_strategy_and_data_recovery&utm_relevant_index=17)  
# 數據治理
[2022 數據治理概念](https://blog.csdn.net/esensoft123/article/details/123866601)  
[2021 數據治理概述](https://blog.csdn.net/wapecheng/article/details/120012702?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167565602116800217045802%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167565602116800217045802&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-30-120012702-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E6%95%B8%E6%93%9A%E8%B4%A8%E9%87%8F%E8%A6%8F%E5%89%87&spm=1018.2226.3001.4449)   
