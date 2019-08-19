# sean 日誌

## 介紹

沒事就來做做看

##成果展示

![](https://github.com/chang0509/sean/raw/master/%E6%9C%AA%E5%91%BD%E5%90%8D.png)

## 使用技巧

名稱    |    說
--------|---------
python  | 不說
Flask   | 幫我架設網站
repl.it | 線上寫程式環境
Heroku | 免費放網站的佛心公司
Github | 真正的佛心企業

## 範例代碼

```python
@app.route("/")
def root():
  ds = glob.glob("articles/*")
  result = []
  for d in ds:
    fs = glob.glob(d + "/*.txt")
    t = (d.split("/")[-1], len(fs))
    result.append(t)
  return render_template("index.html", d = result)
```

## 網址

[請點我](https://elwingdiary.herokuapp.com/)
