## Git & GitHub 操作ガイド

### 1. ローカル環境への複製（クローン）

```bash
# リポジトリをクローン
git clone git@github.com:de-developer-1/git_test.git

# クローンしたディレクトリに移動
cd git-practice
```

### 2. ブランチの作成と切り替え

```bash
# 新しいブランチを作成して切り替え
git checkout -b feature-branch

# 現在のブランチを確認
git branch
```

### 3. ファイルの変更とコミット

```bash
# テキストファイルを作成
echo "# Git練習用ファイル" > sample.txt

# 変更をステージング
git add sample.txt

# 変更をコミット
git commit -m "サンプルファイルを追加"
```

### 4. GitHubへのプッシュ

```bash
# リモートリポジトリに新しいブランチをプッシュ
git push -u origin feature-branch
```

### 5. プルリクエストの作成（GitHub上で）

1. GitHubのリポジトリページを開く
2. 「Compare & pull request」ボタンをクリック
3. プルリクエストのタイトルと説明を入力
4. 「Create pull request」をクリック

### 6. マージ（GitHub上で）

1. プルリクエストページで「Merge pull request」をクリック
2. 「Confirm merge」をクリック
3. ブランチの削除も選択可能

### 7. ローカル環境での更新

```bash
# mainブランチに戻る
git checkout main

# リモートの変更を取得
git pull origin main
```
