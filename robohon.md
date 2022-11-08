# ロボホンに関する調査
目的：ロボホン開発するときに何をやるかを知る

## 開発環境
### RoBoHoN Software Development Kit（RoBoHoN SDK)
- Androidの標準のAPIに加えて、ロボホンのデバイスと音声対話を利用したアプリ開発が可能
- 音声認識の利用回数制限
  - RoBoHoN SDKを利用して開発するアプリ：１か月上限1000回。利用回数が上限に達したら：テキストを利用して、音声入力をエミュレートする手段を用意
- システム要件
  - Android Studio
    - ADB USB DriverはWindows用のみの提供です。Mac OS Xでは必要ない)

### 開発プラットフォーム
- Android Studio(https://developer.android.com/studio)
  - ダウンロード済
  - 続きはまだ：https://mukai-lab.info/pages/tech/robohon/robohon1/

## 資料
https://robohon.com/sdk/develop-list.php

### RoBoHoN_アプリ開発スタートガイド(Version 2.0.0)
- https://robohon.com/assets/sdk/pdf/RoBoHoN_Develop_Start_Guide.pdf

### RoBoHoN_アプリ開発ガイドライン(Version 2.0.0)
- https://robohon.com/assets/sdk/pdf/RoBoHoN_Develop_Guidline.pdf

### RoBoHoN_HVML 2.0 リファレンス(Version 2.0.0)
- https://robohon.com/assets/sdk/pdf/RoBoHoN_HVML_Reference.pdf

### RoBoHoN_アプリ開発用ツール利用手順書(Version 1.0.0)
- https://robohon.com/assets/sdk/pdf/RoBoHoN_DevelopmentTool_Manual.pdf

### Package Index - RoBoHoN API
- https://robohon.com/assets/sdk/javadoc/reference/packages.html


## RoBoHoN_開発者向けモデル＜SR-X002＞
- ロボホンの対話シナリオの作成ができる
- 「Motion Works for ロボホン」（Windows用ソフトウェア）で作成したモーションを生かしたアプリケーションの開発が可能
- Android5.0以上のスマートフォンで、実行させることも可能
### 子供向けのビジュアルプログラミング言語Scratch(スクラッチ)
- スクラッチパック
  - Scratchを使って、ロボホンの対話や機能をプログラミングすることができるアプリケーションパック
  - プログラミングの基礎学習、小中学生のプログラミング教育、家庭などに活用できる
### ロボホンでプログラミング学習
- https://robohon.com/co/scratch.php
1. イメージどおりにロボットがかわいく動くので楽しい
2. 対話シナリオをプログラミングすることができる
3. ロボホン自身がプログラミングの説明をすることができる
4. 小さいので扱いやすい
5. 作ったプログラムはいつでもどこでも再生可能
<img width="690" alt="スクリーンショット 2022-11-08 21 32 05" src="https://user-images.githubusercontent.com/62456878/200564447-4f177f9b-7524-45f7-a37b-c6c659f7cb07.png">

<img width="720" alt="スクリーンショット 2022-11-08 21 32 21" src="https://user-images.githubusercontent.com/62456878/200564502-c660f35c-d580-410a-a44e-bd316035510b.png">

<img width="676" alt="スクリーンショット 2022-11-08 21 32 31" src="https://user-images.githubusercontent.com/62456878/200564538-e29da3c3-4fcb-413c-990d-84041e6559ff.png">

## SDKの紹介
https://robohon.com/sdk/sdk.php
### ロボホン固有の拡張API
- Voice User Interface API
  - 音声対話が主なインターフェース、音声対話を実現するため「音声UI」を組み込んで、それを利用するためのAPI
- ProjectorManager API
  - ロボホンが持つ特徴的なデバイスの一つ：プロジェクター
  - プロジェクターを利用するためのモジュールが組み込んで、このモジュールを利用するためのAPI
- Addressbook API
  - 電話帳 情報（オーナー情報、ロボ情報を含む）を利用するためのAPI

## アプリ開発方法
https://robohon.com/sdk/app.php
### アプリ開発の流れ
#### step1:SDK ダウンロード
#### step2
1. Android Studioのインストール（済）
2. 各種設定と必要なライブラリ登録（↓未完成）
3. ADB Driverのインストール
4. USBデバッグの設定
5. 開発開始Android Studio インストール
#### step3：sample appの使用（ロボホン本体必要）
1. USBで接続
<img width="587" alt="スクリーンショット 2022-11-08 21 51 29" src="https://user-images.githubusercontent.com/62456878/200569050-4215d642-35c4-4e55-8393-f9fe95d3a20c.png">

2. Android Studioでサンプルアプリをインポート
![image](https://user-images.githubusercontent.com/62456878/200569369-19317f9b-c6ab-4690-a914-06e559e9fc48.png)

3. 実行ボタンを押すだけで動かせる
![image](https://user-images.githubusercontent.com/62456878/200569486-5c19cf21-e139-47e5-af05-7c1301d7a1af.png)

4. サンプルアプリを変更して好きなことをしゃべらせる

### サンプルアプリ紹介
- ＳＤＫでは、４つのサンプルアプリを提供
<img width="693" alt="スクリーンショット 2022-11-08 21 54 21" src="https://user-images.githubusercontent.com/62456878/200569871-cc6beef1-8c98-403b-9d1e-61c9ed9fbc9b.png">

### ロボホンの音声対話
- ロボホンの音声対話はクラウドとロボホンの協調で実現
- ロボホンの動作を制御するのがHVML
![image](https://user-images.githubusercontent.com/62456878/200570096-a3304e9f-f70c-416d-9d00-00308c2a563f.png)

### 開発ノウハウ
- ロボホンは音声対話がＵＩの中心となる
  - サンプルアプリ（SampleSimple）をベースに、変えたいところだけ修正していくと、簡単にやりたいことが実現できる
  - **シナリオ作成は、SampleScenario からやりたいことをコピペして作っていくと楽にシナリオが作れる**


