# kids-math — 娘のさんすうアプリ集

GitHub Pages で公開する、子ども向けのさんすうアプリ集です。
1リポジトリに「メニュー（`index.html`）＋ アプリごとのフォルダ」を置く構成。
アプリが増えても **フォルダを1つ足してメニューにカードを1枚追加するだけ** で公開されます。

## 公開URL

- メニュー: `https://<ユーザー名>.github.io/kids-math/`
- 各アプリ: `https://<ユーザー名>.github.io/kids-math/<フォルダ名>/`

iPadの Safari で開き、「共有 → ホーム画面に追加」でアプリ化できます。

## 構成

```
kids-math/
├── index.html              ← アプリを選ぶメニュー画面
├── kazu-no-michi/
│   └── index.html          ← 数直線 ＋ 10のかたまり（位）
└── README.md
```

## 新しいアプリの足しかた

1. 新しいフォルダを作り、その中に `index.html` を置く
   例: `tokei/index.html`
2. ルートの `index.html` のカードのブロックをコピーして、
   `href` のフォルダ名・絵文字・タイトルを差し替える
3. `git add . && git commit -m "add tokei" && git push`
4. 数分後、`.../kids-math/tokei/` で公開される

各アプリの `index.html` は、他に依存しない **単体で完結したHTML** にしておくと管理がラクです。
