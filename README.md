# インストール

`npm install webmerc -g`

# 使い方

### 緯度経度からピクセルを求める

```sh
% webmerc --c2p 35.7,139.7,15
{ x: 7449549.938230911, y: 3302710.99871282 }
```

### ピクセルから緯度経度を求める

```sh
% webmerc --p2c 7449549.938230911,3302710.99871282,15
{ latitude: 139.7, longitude: 35.7 }
```

### 緯度経度からメートルを求める

```sh
% webmerc --c2m 35.7,139.7
{ x: 15551332.863820316, y: 4259419.96554792 }
```

### メートルから緯度経度を求める

```sh
% webmerc --m2c 15551332.863820316,4259419.96554792
{ latitude: 139.7, longitude: 35.7 }
```

### 緯度経度からタイルインデックスを求める

```sh
% webmerc --tileindex 35.7,139.7,15
15/29099/12901
```

# npmモジュール作成手順

### 事前準備

1. npmにsignupして開発者登録しておく
2. `npm adduser`しておく

### 手順

1. `mkdir webmerc`
2. `cd webmerc`
3. `npm init`

    > package.jsonが作成される

4. `npm install`
5. `npm publish`

    > これでnpmに上がる。更新も同じ
