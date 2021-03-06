# DNA-alignment (字串搜尋)

## 目標
    輸入一串以核甘酸ATGC組成的染色體序列，三個為一組基因碼，以ATG為開頭，結束於TAA、TAG或TGA，若序列中
    找不到基因碼則顯示no gene is found

## 條件限制
    1.基因碼為3的倍數
    2.只有1種開頭ATG，結尾有3種TAA、TAG或TGA
    
## 虛擬碼
    1. 輸入字串
    2. 找尋字串ATG開頭
    3. 取得字串長度
    4. 找結尾TAA、TAG、TGA
    5. 算出結尾個數並相加
    6. 判斷頭尾個數是否都大於0
    7. 按字串順序逐一尋找3種結尾
    8. 如果開頭與結尾內是3倍數的基因碼就印出，否則不印
    9. 如果開頭和結尾都沒有，或是有開頭沒結尾、非3倍數長的基因碼，都會印出no gene is found

## 函式
    1. str.split(str="", num=string.count(str))[n:] # 以''內的東西為分隔符號，如果num有指定值，則分割出有num+1個字串的字串陣列，
    取出從第n個索引值到最後的字串.
    2.str.find("") # 找出""內的字符，回傳最先發現的索引值，否則回傳-1
    3.str.count("", start= 0,end=len(string)) # 數""內的字串出現次數

## 結果
![image](https://github.com/leodflag/Python_DNA-alignment/blob/master/DNA_test1.png)
![image](https://github.com/leodflag/Python_DNA-alignment/blob/master/DNA_test2.png)
