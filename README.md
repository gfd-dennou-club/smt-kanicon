# SmT
Matz葉ガニロボコン用のSmT

## How to use
http://kanicon.epi.it.matsue-ct.jp にアクセス

## How to setup

作業ディレクトリの作成
```
$ mkdir SmT
$ cd SmT
```

ソースの取得. ただし，scratch-vm-smt は scratch-vm にリネームする必要がある．
```
$ git clone https://github.com/gfd-dennou-club/smt-gui.git
$ git clone https://github.com/gfd-dennou-club/scratch-vm-smt.git scratch-vm
```
コンパイルと scratch-vm の置換
```
$ cd ~/SmT/scratch-vm
$ npm install
$ sudo npm link

$ cd ~/SmT/smt-gui
$ npm install
$ npm link scratch-vm
```

## How to start
```bash
$ npm start
```
ローカルで実行している場合は，ブラウザで http://localhost:8601 にアクセスする．


## Reference
`smalruby3-gui-smt/`
  * SmT（マイコン制御できるSmalruby）
  * https://github.com/gfd-dennou-club/smalruby3-gui-smt

`scratch-vm/`
  * https://github.com/gfd-dennou-club/scratch-vm-smt
