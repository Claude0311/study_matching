# study_matching留學配對
評分機制：
* 同樣學位+1.5分
* 同樣領域+2分
* gpa + 1/(abs(a-b)+1)

用hungarian algorithm使分數總和最大
## init
```
pip install numpy
pip install pandas
```
## run
```
python ./matching.py ./senior.xlsx ./junior.xlsx
```
### note
xlsx rules:
* senior.xlsx必要欄位
  * 姓名
  * 學位(以' + '區分)
  * 領域(以', '區分)
  * 成績
  * 電子郵件地址
  * 數量
* junior.xlsx必要欄位
  * 姓名
  * 學位
  * 領域
  * 您的Email (必填)
  * 學號
  * 成績
## output
output.csv
* 學長姊姓名
* 學長姊信箱
* 學弟妹姓名
* 學弟妹學號
* 學弟妹信箱
