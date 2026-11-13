# 買取らぼらとり 買取率の推移（公開用）

買取らぼらとりのランキングページ（https://kaitori-laboratory.com/giftcard-ranking）の「買取率の推移」のグラフが読むデータ。

- `rate-history.json`：お魚通販.com グループのサイトの、日ごとの買取率の最高・平均・最低。
- 毎日の記録（非公開のリポジトリ kaitori-lb-rate-log）が、記録のたびに書き換える（1 日 3 回）。手で直さない。
- 率は設定の値（クーポンの上乗せ前）。`rate_up` が上乗せの分で、画面では足して出す。
- グループの集計だけを置く。サイトごとの値や他社の記録は置かない。

記録したデータはお魚通販.com 株式会社のもの。

## 形

```json
{
  "generated_at": "最後の記録の取得日時（日本時間）",
  "group_daily": [
    { "date": "2026-10-16", "sites": 26,
      "max_first": 92, "avg_first": 92, "min_first": 92,
      "max_repeat": 91, "avg_repeat": 91, "min_repeat": 91,
      "rate_up": 1 }
  ]
}
```

読み出す URL：`https://raw.githubusercontent.com/araimotoki0/kaitori-lb-rate-public/main/rate-history.json`
