# lol_settings

## 「プレイヤー移動攻撃のクリック」と「プレイヤー移動攻撃」両方に「Shift + MB2（右クリック）」を設定する方法
- この設定をするとShiftでアタックムーブしながら攻撃範囲を見ることができます
- 利点
    - 射程ギリギリでの攻撃ができる
    - 集団戦で自分を見失いにくくなる
- ![image](https://github.com/user-attachments/assets/e87e3b71-158f-4ce3-8712-97a4f413caa5)
- ![image](https://github.com/user-attachments/assets/616cf9d0-0fde-466d-b717-6213bf1a7189)

## 設定方法
1. lolクライアントを起動してログインまでする
2. `C:\Riot Games\League of Legends\Config\PersistedSettings.json` エディタで開く
3. ファイルから「evtPlayerAttackMoveClick」の「{から},」までを削除（プレイヤー移動攻撃のクリック）
    - ![image](https://github.com/user-attachments/assets/f7230765-6214-4b26-bae1-8ac24640b1d4)
4. プラクティスモードを起動
5. 設定画面を開く
    - 「プレイヤー移動攻撃のクリック」は自動的に「Shift + MB2（右クリック）」に戻る
    - 多分内部的には初期化状態
6. 設定変更で「プレイヤー移動攻撃」にも「Shift + MB2（右クリック）」を設定
7. 以降ファイルの編集は不要、ただしサモリフに入るたびに設定画面から「プレイヤー移動攻撃」にも「Shift + MB2（右クリック）」を設定する必要がある

## 注意点
- 多分「プレイヤー移動攻撃のクリック」を手動設定してしまうともう一度初期化するためにファイルから「evtPlayerAttackMoveClick」を削除するところからやり直しになる

## Appendix

### 複数アカウントを持っており設定を使いまわしたい場合
- 設定の元となるアカウントでlolにログイン
- `C:\Riot Games\League of Legends\Config\PersistedSettings.json`をローカルに保存
- lolクライアントからログアウト
- 別アカウントでlolにログイン
- ローカルに保存した`C:\Riot Games\League of Legends\Config\PersistedSettings.json`を上書き保存
- これでプラクティスモードに入れば同じ設定になる
