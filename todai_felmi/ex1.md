# 日本にぬいぐるみはいくつあるか

## 前提確認
- 個人レベル（店の在庫は含まない）
- 小さいものから大きいものまで

## アプローチ設定
日本のぬいぐるみの数=人口×所有率×一人当たり所有数

## モデル化
- 男女で異なる
- 年齢で異なる

人口
- 12000万人
- 蛸壺のピラミッド
- 0~20: 2400万人
  - 5歳分で600万人
  - 10歳分で1200万人
- 20~40: 3600万人
- 40~60: 3600万人
- 60~80: 2400万人  

所有率, 個数, 人口

| **-**  | **0**             | **5**             | **10**            | **20**            | **30**            | **40**            | **50**            | **60** | **70** |
|--------|-------------------|-------------------|-------------------|-------------------|-------------------|-------------------|-------------------|--------|--------|
| **男** | 50%, 2個, 300万人 | 20%, 2個, 300万人 | 10%, 2個, 600万人 | 10%, 1個, 900万人 | 10%, 1個, 900万人 | -                 | -                 | -      | -      |
| **女** | 80%, 4個, 300万人 | 60%, 3個, 300万人 | 40%, 2個, 600万人 | 30%, 2個, 900万人 | 30%, 1個, 900万人 | 20%, 1個, 900万人 | 10%, 1個, 900万人 | -      | -      |

300+120+120+90+90+960+540+480+540+270+180+90=720+1980+1080=3780万個
