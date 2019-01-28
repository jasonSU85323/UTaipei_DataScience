youtube推薦系統分析
====================
#### 介紹
為了在社群媒體(Youtube)中脫穎而出，除了要有夠好的創意之外，曝光也很重要，如何能夠接觸到觀眾，和理解社群媒體自身的演算法很有關！

- 觀眾想看的是什麼？
- 現在的流行趨勢是什麼？
- 創作者現在要做的又是什麼？

#### 資料集來源
- kaggle：Trending YouTube Video Statistics
- Link：https://www.kaggle.com/datasnaek/youtube-new
- 以「US」探討對象

#### 資料集欄位
|   |名稱   |描述   |
| :------------: | ------------ | ------------ |
|1 |video id |視頻ID|
|2 |trending date|發燒日期|
|3 |title |視訊名稱|
|4 |channel title|頻道名稱|
|5 |category id|類別ID|
|6 |pulish time|上傳日期|
|7 |tags|標籤|
|8 |views|觀看次數|
|9 |likes|喜歡|
|10|dislikes|不喜歡|
|11|comment count|評論數|
|12|thumbnail link|縮略圖鏈接|
|13|comments disabled|評論已禁用(TRUE/FLSE)|
|14|ratings disabled|評級(TRUE/FLSE)|
|15|video error or removed|視頻錯誤或已刪除(TRUE/FLSE)|
|16|description|描述

#### 問題定義
1. 各類別影片 - 觀看次數 & 喜歡 & 不喜歡 『有正關係??』
2. 各影片觀看次數區間 - 喜歡 & 不喜歡 & 留言數 『有正關係??』
3. 影片的標題是否關鍵？
4. 所有影片 - 標籤數 & 觀看次數 『有正關係??』
5. 影片下方詳細文字中有否YouTube的連結 & 觀看次數 『有正關係??』
6. 發燒影片中時間區間內是有特定幾種影片種類的！

#### 結果