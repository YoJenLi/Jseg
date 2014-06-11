<h1>Jseg</h1>
<h2>A modified version of <a href="https://github.com/fxsjy/jieba">Jieba</a> segmentator</h2>

<h3>Synopsis</h3>

<h3>Usage</h3>
```
from Jseg import jieba

```
Here's a sample text:
```
sample = '''台灣大學語言學研究所LOPE實驗室超強
            Taco門神超罩
            Amber 和 Emily 是雙胞胎 
            期末要爆炸啦！ ◢▆▅▄▃崩╰(〒皿〒)╯潰▃▄▅▇◣
         '''
```
Segmentation
```
result = jieba.seg(sample)
```
Output
```
print result.text()

台灣/Nca 大學/Ncb 語言學/Nad 研究所/Ncb LOPE/FW 實驗室/Ncb 超強/VH11 
Taco/FW 門神/Nad 超罩/VH14 
Amber/FW 和/Caa Emily/FW 是/V_11 雙胞胎/DM 
期末/Ng 要/Dbab 爆炸/VH11 啦/Tc ！/PUNCTUATION ◢▆▅▄▃崩╰(〒皿〒)╯潰▃▄▅▇◣/EMOTICON
```