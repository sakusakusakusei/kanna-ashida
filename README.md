# 芦田かんな オフィシャルサイト

ヴィブラフォン・打楽器奏者 芦田かんな のオフィシャルホームページです。

---

## ファイル構成

```
/
├── index.html       # サイト本体（画像・動画すべて埋め込み済み）
└── README.md        # このファイル
```

`index.html` 1ファイルにすべてのコンテンツ（プロフィール写真・背景画像・スタイル・スクリプト）が含まれています。

---

## 公開URL

GitHub Pages で公開中：  
`https://<username>.github.io/<repository-name>/`

---

## スケジュールの更新方法

`index.html` をテキストエディタ（VS Code 推奨）で開き、  
**`<!-- UPCOMING -->`** または **`<!-- PAST -->`** を検索してください。

### 次回公演を更新する

`<!-- UPCOMING -->` のブロック内にあるカードを編集します。

```html
<a class="live-upcoming-card reveal" href="公演ページのURL" target="_blank" rel="noopener">
  <div class="luc-left">
    <span class="luc-date">2026.06.13 (Sat) / 06.14 (Sun)</span>
    <h3 class="luc-title">公演タイトル</h3>
    <p class="luc-subtitle">サブタイトル（不要なら行ごと削除）</p>
    <p class="luc-venue">会場名</p>
    <ul class="luc-details">
      <li>開演時間</li>
      <li>料金</li>
      <li>定員・備考</li>
    </ul>
  </div>
  <div class="luc-right">
    <span class="luc-tag">Recital</span>
    <span class="luc-arrow">→</span>
  </div>
</a>
```

### 公演が終わったら

1. Upcoming のカードを削除（または次の公演に差し替え）
2. 下記テンプレートを `<!-- PAST -->` のブロック先頭にコピペして追加

**リンクあり**
```html
<a class="live-item live-past reveal" href="URL" target="_blank" rel="noopener">
  <span class="live-date">YYYY.MM</span>
  <div>
    <p class="live-title">公演タイトル</p>
    <p class="live-venue">会場名</p>
  </div>
  <span class="live-tag">Recital</span>
</a>
```

**リンクなし**
```html
<div class="live-item live-past reveal">
  <span class="live-date">YYYY.MM</span>
  <div>
    <p class="live-title">公演タイトル</p>
    <p class="live-venue">会場名</p>
  </div>
  <span class="live-tag">Recital</span>
</div>
```

### live-tag の種類

| タグ名 | 用途 |
|--------|------|
| `Recital` | ソロリサイタル |
| `Duo Recital` | デュオリサイタル |
| `Ensemble` | アンサンブル・室内楽 |
| `Orchestra` | オーケストラ共演 |
| `Festival` | 音楽祭 |
| `Premiere` | 初演 |
| `Performance` | その他パフォーマンス |

---

## お問い合わせフォーム

[Formspree](https://formspree.io) を使用しています。  
送信されたメッセージは登録メールアドレスに届きます。

---

## 使用フォント（Google Fonts）

| フォント | 用途 |
|----------|------|
| Shippori Mincho | 名前（芦田かんな） |
| Noto Serif JP | 本文 |
| Cormorant Garamond | 英字見出し |
| DM Mono | ラベル・番号 |

---

## SNSリンク

変更する場合は `index.html` 内の以下を検索してください。

```
https://www.instagram.com/_gqunq/
https://www.youtube.com/@kannaashida
https://x.com/gqunq
```

---

## 技術仕様

- 静的HTML（サーバー不要）
- 外部依存：Google Fonts / Formspree のみ
- 対応：PC・スマートフォン（レスポンシブ対応）
