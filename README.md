# myMemo
## GitHub利用について、
2021年8月にパスワード認証によるリモートアクセスの廃止されアクセストークンが必要に。

アクセストークンの設定方法は、Settings -> Developer settings -> Personal Access Tokens

fine-grainedなアクセストークンはまだbeta版。

## アクセストークン(classic)の設定(以下の項目にチェックを入れる)
1.repo

2.workflow

3.user

4.write:discussion

5.admin:enterprise

6.admin:gpg_key

## アクセストークンを用いたコミットとpush(Prismoidはユーザー名)
```
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://Prismoid:[アクセストークン]@github.com/Prismoid/test.git
git push -u origin main
```

## github 設定確認用コマンド
```
color.ui : Gitの出力の色分け（通常はautoと設定）
core.editor : コミットメッセージなどの編集で用いるエディタ
user.name : ユーザー名 -> メールアドレスが入っている
user.email : Eメールアドレス
```