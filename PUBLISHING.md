# 配布用リポジトリ運用メモ（メンテナ向け）

このリポジトリは **公開配布専用**です。
大容量の配布ZIPは **gitにコミットせず**、GitHub Release の Assets に添付して配布します。

## 1. GitHubでリポジトリを作成

- GitHub → New repository
- Name: `Dungeon_of_the_Living_Will-Releases`
- Visibility: Public
- Initialize: どちらでもOK（READMEは後でpushでも良い）

## 2. このフォルダを push

このワークスペースには雛形が `./_release_repo/Dungeon_of_the_Living_Will-Releases/` にあります。

例（PowerShell）:

```powershell
Set-Location D:/projects/Dungeon_of_the_Living_Will/_release_repo/Dungeon_of_the_Living_Will-Releases

git init
# 既存のデフォルトブランチ名に合わせる（main推奨）
git checkout -b main

git add -A
git commit -m "chore: initial release repo"

git remote add origin https://github.com/<owner>/Dungeon_of_the_Living_Will-Releases.git
git push -u origin main
```

## 3. GitHub Release を作成して ZIP を添付

- Releases → Draft a new release
- Tag: `v0.1.0`（例）
- Title/Notes: 用意したリリースノートを貼り付け
- Assets: `Dungeon_of_the_Living_Will_*.zip` を **Upload**

※ ZIPはリポジトリにコミットせず、Releaseページに添付する運用にします。
