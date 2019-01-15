# 數據分析
====================
在免費的app中，篩選平均用戶評分值為 0 & 5 的app在依照他的主要類型做計數，分析其關係。


* 資料來源
	* https://www.kaggle.com/ramamet4/app-store-apple-data-set-10k-apps

* appleStore.csv
	* id：應用程序ID
	* track_name：應用名稱
	* size_bytes：大小（以字節為單位）
	* currency：貨幣類型
	* price：價格金額
	* rating_count_tot：用戶評分計數（適用於所有版本）
	* rating_count_ver：用戶評分計數（當前版本）
	* user_rating：平均用戶評分值（適用於所有版本）
	* user_rating_ver：平均用戶評分值（對於當前版本）
	* ver：最新版本代碼
	* cont_rating：內容評級
	* prime_genre：主要類型
	* sup_devices.num：支持設備的數量
	* ipadSc_urls.num：顯示的屏幕截圖數量
	* lang.num：支持的語言數量
	* vpp_lic：啟用基於Vpp設備的許可

* appleStore_description.csv
	* id：應用程序ID
	* track_name：應用程序名稱
	* size_bytes：內存大小（以字節為單位）
	* app_desc：應用程序說明