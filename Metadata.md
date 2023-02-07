
# Metadata
範圍將涵括數據產生、數據存儲、數據加工和展現等各個環節的數據描述信息，幫助用戶理解數據來龍去脈、關係及相關屬性。按其描述對象分三類: 
1. 業務 Business Metadata: 據包括主題域、業務規則、隱私級別、定義、術語表、運算法則和系統使用業務語言等。
2. 技術 Technical Metadata: 數據的系統表(存放位置)和字段結構、屬性(存儲類型)、出處、依賴性(血緣關係)等等。
3. 操作 Operational Metadata: 頻率、記錄數以及各個組件的分析和其它統計信息等。

### 元數據有什麼用？ 
假設你在管理報表，有一天你發現有報表數據中指標3 的數據異常，你需要找出錯誤的數據並提交流程修正，那麼這個錯誤數據從何而來？一個個核對數據顯然不夠高效，那你就得知道這個報表的的指標來源，元數據的血緣分析能幫助你分析這個錯誤數據的上游路徑。  
查看元數據可以發現：指標3 是由數據集市的B主題數據經過ETL過程生成的，B主題數據又是由數據倉庫中的table1 和table 4經過ETL過程生成的。  
![image](https://user-images.githubusercontent.com/117702322/217144582-1d9b0452-b20e-4881-a891-373c852fcc20.png)

## 元數據分層
元數據管理平台: 元數據管理工具是否強大部分體現在其對各類數據源的採集能力上。  
![image](https://user-images.githubusercontent.com/117702322/217145993-be3a0bf6-0435-43a8-acf9-4b91c2a10156.png)  

[2022 用友團隊:元數據說明書](https://blog.csdn.net/hzbooks/article/details/124287779?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167574109616800211560006%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=167574109616800211560006&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-124287779-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E5%85%83%E6%95%B8%E6%93%9A%E5%B1%A4&spm=1018.2226.3001.4187)  
[2022 數據元、元數據、主數據、參考數據概述](https://blog.csdn.net/qq_41116027/article/details/124392461?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167574109616800211531216%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167574109616800211531216&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-5-124392461-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E5%85%83%E6%95%B8%E6%93%9A%E5%B1%A4&spm=1018.2226.3001.4187)    
[2022 元數據中心的關鍵目標和技術實現方案](https://blog.csdn.net/m0_54252387/article/details/125544340?ops_request_misc=&request_id=&biz_id=102&utm_term=%E5%85%83%E6%95%B8%E6%93%9A%E5%B1%A4&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-6-125544340.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&spm=1018.2226.3001.4187)  
