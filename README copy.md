# フォーク元からの更新作業
## フォーク元リポジトリをリモートに追加
git remote add upstream https://github.com/tegnike/aituber-kit.git

## リモートの確認
git remote -v

## フォーク元リポジトリから最新の変更をフェッチ
git fetch upstream

## ローカルのメインブランチを最新化
git checkout main
git merge upstream/main

## （必要な場合）コンフリクトの解決
## コンフリクトを解決したら、変更をコミット
git add .
git commit -m "Resolved merge conflicts"

## 自分のリモートリポジトリにプッシュ
git push origin main

-----------------------------------------

## 起動

## パッケージインストールします。
npm install

## 開発モードでアプリケーションを起動します。
npm run dev
