# houransai-web

芳藍祭2027年度のwebサイト用のリポジトリです。(11月22日開始)

## 運用マニュアル

### 前提

- VScodeをダウンロードしておくこと

### 1. リポジトリ（ファイル）をクローンする

1. VScodeを開く
2. cmd + Jでターミナルを開く
3. ターミナルでリポジトリを保存したい場所に移動する（例desktop）  
   `cd ~/Desktop`
4. 以下のコマンドでリポジトリをクローンする  
   `git clone https://github.com/houransai-develop/houransai-web.git`
5. クローンしたリポジトリをVScodeで開く  
   `cd houransai-web`  
   `code .`

### 2. Push（変更をGitHubに反映する）方法

1. VScodeで変更を加える
2. 変更を保存する（cmd + S）
3. ターミナルを開く（cmd + J）
4. 変更をGitHubにプッシュする  
   `git add .`  
   `git commit -m "ここで変更内容を簡潔に書く"`  
   `git push`
5. 最新ではない状態で編集しpushした時にエラーが出た場合
   `git commit -m "ここで変更内容を簡潔に書く"` の後に
   `git pull --rebase origin main`
　　`git push origin main`
  
### 3. Pull（他の人の変更をローカルに保存）する方法

5. ターミナルを開く（cmd + J）
6. 以下のコマンドでリモートリポジトリの変更をローカルに反映する  
   `git switch main`  
   `git pull origin main`
