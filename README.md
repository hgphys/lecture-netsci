# 体験授業：「つながり」のデータサイエンス

金沢学院大学 情報工学部　後藤弘光

Python のネットワーク分析ライブラリ [NetworkX](https://networkx.org/) を使って、有向グラフを定義・可視化し、各ノードの **PageRank** を計算してみる体験プログラムです。高校生・初学者向けに、ブラウザだけで動かせるように作っています。

---

## 体験内容

- 有向グラフ（向きのあるつながり）を自分で定義する
- グラフを可視化する
- 各ノードの PageRank を計算し、重要度を色の濃さで可視化する

PageRank は Google の検索エンジンでも使われている、ネットワーク上の「重要さ」を測る指標です。SNS のフォロー関係、Web ページのリンク関係、論文の引用関係など、身の回りの「つながり」の分析にも応用できます。

---

## 使い方

### ブラウザだけで体験する（推奨）

下のボタンから Google Colab で開けます。Google アカウントがあればインストール不要で実行できます。

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hgphys/lecture-netsci/blob/main/NetSci_PageRank.ipynb)

1. 上のボタンをクリックして Colab で開く
2. 左上の「ファイル」→「ドライブにコピーを保存」を選択
3. セルを上から順番に実行（▶ ボタンまたは `Shift + Enter`）
4. `edge = ["a","c"]` の部分を書き換えて、自分の好きなつながりを作ってみよう

### 自分のパソコンで動かす場合

```bash
git clone https://github.com/hgphys/lecture-netsci.git
cd lecture-netsci
pip install networkx numpy matplotlib jupyter
jupyter notebook NetSci_PageRank.ipynb
```

---

## ファイル構成

```
lecture-netsci/
├── NetSci_PageRank.ipynb   # 体験用ノートブック
└── README.md
```

---

## 関連リポジトリ

大学での発展的な内容に興味のある方は、こちらもご覧ください。

- [ネットワーク科学と経済 I](https://github.com/hgphys/ns1) — グラフ理論の基礎、次数分布、スモールワールド
- [ネットワーク科学と経済 II](https://github.com/hgphys/ns2) — リンク予測、コミュニティ検出、二部グラフ

---

## License

This work is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
