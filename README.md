# hatagayatei.com 追加ページ一式

既存のページを壊さず、トップページ・一覧ページ・活動導線ページを追加するための静的HTML一式です。

## 追加される主なページ

- `/` トップページ
- `/doujinshi/` 同人誌・ZINE一覧
- `/doujinshi/silo/` サイロを嫌う
- `/doujinshi/tsukuru-mae-ni-tsukawarekata/` 作る前に使われ方を考える
- `/doujinshi/ai-foreshadowing/` AIという名の伏線回収
- `/doujinshi/genjitsu-karano-sukoshi-no-choyaku/` 現実からの少しの跳躍
- `/talks/` 登壇
- `/communities/` コミュニティ
- `/communities/tamadev/` 多摩.dev
- `/communities/hadano-agile/` 秦野アジャイル
- `/communities/kosodate-engineering/` 子育てエンジニアリングMeetup
- `/music/` 音楽作品一覧
- `/404.html` 404ページ
- `/style.css` 共通CSS

## 既存ページについて

次の既存ページは同梱していません。上書きせず、一覧ページからリンクする前提です。

- `/doujinshi/penguin-frog/`
- `/music/asagayaladymadonna/`
- `/music/yoru-ni-odoreba/`

## GitHub Pages への反映例

既存リポジトリのルートで、zipを展開した中身をコピーします。

```bash
cp -R /path/to/hatagayatei-site-additions/. .
git status
git add .
git commit -m "Add site index and activity archive pages"
git push
```

## 調整したほうがよい箇所

- `doujinshi/genjitsu-karano-sukoshi-no-choyaku/` のタイトル・ページ数・初出は、手元の入稿情報に合わせて確認してください。
- 各作品ページに表紙画像を置く場合は、`assets/` 配下に画像を追加し、各HTMLに `<img>` を足す想定です。
- Speaker Deckやブログ記事への個別リンクは、必要に応じて `/talks/` に追加してください。
