# lol_settings

## Shiftアタックムーブでも攻撃範囲を表示する方法
- この設定をするとShiftでアタックムーブしながら攻撃範囲を見ることができます
- 利点
    - 射程範囲表示のアタックムーブをするのに右クリックのみで行える
    - 射程ギリギリでの攻撃ができる
    - 集団戦で自分を見失いにくくなる
- 以下のような設定をします
    - ![image](https://github.com/user-attachments/assets/e87e3b71-158f-4ce3-8712-97a4f413caa5)
    - ![image](https://github.com/user-attachments/assets/616cf9d0-0fde-466d-b717-6213bf1a7189)

## 注意
- サモリフに入るたびに以下の手順が必要です
    - 設定を開く
    - 「プレイヤー移動攻撃」をバインド解除
    - 「プレイヤー移動攻撃」に「Shift + MB2（右クリック）」を設定

## 上記設定ができない場合
- 「プレイヤー移動攻撃のクリック」を一度でも手動で設定したことがある場合同じボタンを設定することができなくなります
- その場合は以下の手順を行うことで設定可能です
1. lolクライアントを起動してログインまでする
2. `C:\Riot Games\League of Legends\Config\PersistedSettings.json` エディタで開く
3. ファイルから「evtPlayerAttackMoveClick」の「{から},」までを削除（プレイヤー移動攻撃のクリック）
    - ![image](https://github.com/user-attachments/assets/f7230765-6214-4b26-bae1-8ac24640b1d4)
4. プラクティスモードを起動
5. 設定画面を開く
    - 削除した「プレイヤー移動攻撃のクリック」は自動的に復活して「Shift + MB2（右クリック）」に戻ります
    - 多分内部的には初期化状態
6. 設定変更で「プレイヤー移動攻撃」に「Shift + MB2（右クリック）」を設定
7. 以降ファイルの編集は不要です

## Appendix

### 複数アカウントを持っており設定を使いまわしたい場合
- 設定の元となるアカウントでlolにログイン
- `C:\Riot Games\League of Legends\Config\PersistedSettings.json`をローカルPCに保存
- lolクライアントからログアウト
- 別アカウントでlolにログイン
- ローカルPCに保存した`PersistedSettings.json`を以下に上書き保存
    - `C:\Riot Games\League of Legends\Config\PersistedSettings.json`
- プラクティスモードに入って動作確認
