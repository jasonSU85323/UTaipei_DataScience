※ youtube 推薦系統分析		

index：
USvideos.csv		-> 原始檔
US_category_id.csv	-> label表
newtest.csv		-> 整理後


1	video id		視頻ID
2	trending date		
3	title			視訊名稱			*
4	channel title		頻道名稱			*
5	category id		類別ID				*
6	publish time		上傳日期
7	tags			標籤
8	views			觀看次數			*
9	likes			喜歡				*
10	dislikes		不喜歡				*
11	comment count		評論數				*
12	thumbnail link		縮略圖鏈接
13	comments disabled	評論已禁用(TRUE/FLSE)
14	ratings disabled	評級(TRUE/FLSE)
15	video error or removed	視頻錯誤或已刪除(TRUE/FLSE)
16	description		描述				*

$3 "," $4 "," $5 "," $8 "," $9 "," $10 "," $11 "," $16

--------------------------
echo title,channel title,category id,views,likes,dislikes,comment count,description >> newtest.csv
cat USvideos.csv | awk -F, '{if($5 ~ /^[0-9]+$/ && $5 < 45 ) print $3 "," $4 "," $5 "," $8 "," $9 "," $10 "," $11 "," $16;}' >> newtest.csv
cat newtest.csv | awk -F, '{print $3}' | sort | uniq -c
   2116 1
   5679 10
    819 15
   1809 17
    353 19
    312 2
    777 20
   2897 22
   3313 23
   9266 24
   2138 25
   3995 26
   1564 27
   2180 28
     53 29
     57 43