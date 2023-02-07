
## 數據倉儲分層
1. ODS原始數據: 存放原始數據，直接加載原始日誌、數據，數據保持原貌不做處理。
2. DW 數據倉庫: 中間層數據。  

    - DWD(Detail)明細數據層：對ODS層數據進行清洗、去除離群脫敏等。保存明細數據，一行信息代表一次業務行為，例如一次下單。    
    - DWS(Service)服務數據層：以DWD為基礎，按天進行輕度匯總。一行信息代表一個主題一天的總行為，例如一個用戶一天下單次數。  
    - DWT(Topic)服務主題層：以DWS層為基礎，對數據進行累積匯總。一行信息代表一個主題的累積行為，例如一個用戶從註冊那天開始至今一共下了多少次單。  

3. DA 數據應用: 面向業務定制，各種統計報表。
※ DIM 維度層
![image](https://user-images.githubusercontent.com/117702322/217148035-910b18f4-8bfb-4aec-88a9-c2ebcac7b79f.png)

[2021 數倉分層架構及三層架構流程](https://blog.csdn.net/xianyu120/article/details/117374469?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167574109616800211531216%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=167574109616800211531216&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-10-117374469-null-null.142^v73^control,201^v4^add_ask,239^v1^insert_chatgpt&utm_term=%E5%85%83%E6%95%B8%E6%93%9A%E5%B1%A4&spm=1018.2226.3001.4187)  
[2021 電商數倉數據採集](https://blog.csdn.net/FunnyPrince_/article/details/120339260?spm=1001.2101.3001.6650.10&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EOPENSEARCH%7ERate-10-120339260-blog-117888317.pc_relevant_multi_platform_whitelistv3&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EOPENSEARCH%7ERate-10-120339260-blog-117888317.pc_relevant_multi_platform_whitelistv3&utm_relevant_index=11)    
