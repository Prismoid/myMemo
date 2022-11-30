# myMemo
## GitHub利用について、
### 2021年8月にパスワード認証によるリモートアクセスの廃止
### アクセストークンが必要に。
### 設定方法は、Settings -> Developer settings -> Personal Access Tokens

## アクセストークンを用いたコミットとpush(Prismoidはユーザー名)
### git init
### git add README.md
### git commit -m "first commit"
### git branch -M main
### git remote add origin https://Prismoid:[アクセストークン]@github.com/Prismoid/test.git
### git push -u origin main
