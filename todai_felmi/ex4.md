# 日本に郵便ポストはいくつあるか？
## 前提確認
- 赤いやつ
## アプローチ設定
- 面積×ポスト１つあたりの面積
## モデル化
- 日本は面積38万km2
- 山地と平地に分類
  - 山地が3/4
    - 1/3が無人地域
    - 2/3が有人地域→時速4kmで歩いた時、30分で着く→2km四方→1個/4km2
  - 平地が1/4→時速4kmで歩いた時、15分で着く→1個/1km2
## 計算実行
- 山地かつ有人地域の面積/4：38×(3/4)×(2/3)/4=4.75  
- 平地の面積/1：38×(1/4)=9.5  

**合計14万個**
