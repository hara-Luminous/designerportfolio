# Portfolio CMS Prototype

GitHub Pages でそのまま公開できる構成です。

## 公開方法

1. GitHub で新しいリポジトリを作成
2. このフォルダ内のファイルをすべてリポジトリ直下にアップロード
3. GitHub の `Settings` → `Pages`
4. `Build and deployment` の Source を `Deploy from a branch` に設定
5. Branch を `main`、Folder を `/(root)` にして Save
6. 数分後に GitHub Pages のURLが発行されます

## ファイル構成

- `index.html` : 公開サイト + 管理画面
- `assets/` : 初期作品画像
- `.nojekyll` : GitHub Pages用
- `README.md` : この説明

## 重要

現在の管理画面は `localStorage` を使用しています。

そのため、GitHub Pages上でも
- 画像追加
- タイトル編集
- カテゴリー編集
- タグ編集
- 備考編集
- 公開 / 非公開
- 並び替え

は動作しますが、変更内容は「操作したブラウザ内」にだけ保存されます。

GitHub リポジトリ自体へ新しい画像や作品データを書き込む機能はまだありません。
複数PCで共通管理したい場合は Supabase 等のバックエンド連携版に変更してください。
