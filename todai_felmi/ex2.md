# 日本に自動車は何台あるか？
## 前提確認
- 自家用と業務用あるが、自家用のみで考える。
## アプローチ設定
- 自動車数=世帯数×所有率×所有数
## モデル化
- 都会と田舎で分類する
- 世帯で考える。世帯ごとに車を所有するため。
  - 都会の平均世帯人数:2人→3000万世帯と仮定
  - 田舎の平均世帯人数:3人→2000万世帯と仮定
- 単身世帯と複数世帯で所有率・数が異なる
  - 単身の場合、男女で所有率が異なる

中の数値は、世帯の割合, 世帯数, 所有率, 所有数
  
| -                | 単身世帯(男)            | 単身世帯(女)           | 複数世帯                 |
|------------------|---------------------|--------------------|----------------------|
| 都会(3000万世帯) | 20%, 600万世帯, 40%, 1.1台/世帯 | 10%, 300万世帯, 10%, 1.1台/世帯 | 70%, 2100万世帯, 70%, 1.5台/世帯 |
| 田舎(2000万世帯) | 15%, 300万世帯, 80%, 1.2台/世帯 | 5%, 100万世帯, 50%, 1.2台/世帯  | 80%, 1600万世帯, 90%, 1.8台/世帯 |

## 計算  
表の中身を計算
| -                | 単身世帯(男)            | 単身世帯(女)           | 複数世帯                 |
|------------------|---------------------|--------------------|----------------------|
| 都会(3000万世帯) | 264 | 33 | 2205 |
| 田舎(2000万世帯) | 288 | 60 | 2592 |

合計で5442万台




