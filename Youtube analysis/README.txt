�� youtube ���˨t�Τ��R		

index�G
USvideos.csv		-> ��l��
US_category_id.csv	-> label��
newtest.csv		-> ��z��


1	video id		���WID
2	trending date		
3	title			���T�W��			*
4	channel title		�W�D�W��			*
5	category id		���OID				*
6	publish time		�W�Ǥ��
7	tags			����
8	views			�[�ݦ���			*
9	likes			���w				*
10	dislikes		�����w				*
11	comment count		���׼�				*
12	thumbnail link		�Y�����챵
13	comments disabled	���פw�T��(TRUE/FLSE)
14	ratings disabled	����(TRUE/FLSE)
15	video error or removed	���W���~�Τw�R��(TRUE/FLSE)
16	description		�y�z				*

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