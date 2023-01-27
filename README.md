# Creative.hack_2022  
2022年度下期Creative.hack作業用リポジトリ  
作業者：齋藤、伊藤、もちまる  
テーマ：Twitterのバズり予測（仮）

## 目次
1. [Githubの使い方](#Github)

<a id='Github'></a>

## Github使い方まとめ

### Githubでコードを管理するにあたっての注意事項
- main（master）ブランチで直接操作をしない
- 1つのファイルのサイズが100MByteになるように
- 複数人で同じブランチを操作しない
複数人が同じブランチに対してpushすると、先にpushした方の編集内容が上書きされて消えてしまうため。（そもそもGitがエラー吐くと思う）
- 違うブランチでも同じファイルを編集しない
やったことないから分からないけど、多分片方の編集内容が上書きされて面倒なことになる

### Githubでよく使うコマンド

#### リモートブランチをローカルにクローンする際
git clone コマンド
```
git clone https://github.com/k-saito0107/Creative.hack_2022.git
```
#### ブランチの作成・切り替え・確認

##### ブランチの切り替え
git checkout コマンド
```
# <branchname>ブランチに切り替え
git checkout <branchname>
```

##### ブランチの作成
1. git branch コマンド
```
# <branchname>ブランチを作成
git branch <branchname>
```

2. git checkout -b コマンド
git checkout -b とすると、新しいブランチを作成するとともに、作成したブランチに切り替えることができる。
```
# <branchname>ブランチを作成し、作成したブランチに切り替える
git checkout -b <branchname>
```

##### ブランチの確認
git branch -aとすると現在入っているブランチを確認できる。
```
git branch -a

#main
#* saito
#  remotes/origin/HEAD -> origin/main
#  remotes/origin/main
#  remotes/origin/saito
```

