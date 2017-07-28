# TangoAR
Unity and Google Tnago Project

## 開発環境
* Unity 2017.1.0f3 (64-bit)
* Tango SDK for Unity
* Visual Studio 2017

## 導入方法
* **Unity**を`Visual Studio 2017 Tools for Unity Package`にチェックを入れてインストール
* Visual Studio Installerを開き、インストール済みのVisual Studioの`変更`→`ワークロード`から`C++によるモバイル開発`を選択し、**Android SDK**や**JDK**をインストール
* Unityに新規3D Projectを作成後、**Google Tango SDK**のパッケージを作成したプロジェクトにインストール

## 環境設定
* パス周りはVisual Studio InstallerでAndroid SDKをインストールした際にほとんど設定がなされているので省略
* Unityで`File`→`Build Settings`→`Android`を選択し`Switch Platform`でビルド対象をAndroidに設定
* `Player Settings...`からアンドロイドマークをクリックし、`Other Settings`→`Package Name`を`com.unity3d.[アプリ名]`に変更
* `Other Settings`→`Minimum API Level`を`Android 4.2 'Jelly Bean'(API Level 17)`に設定
* Unityで`Edit`→`Preferences`→`External Tools`からAndroid SDKとJDKのインストール場所を指定する
* Unity Projectをバージョン管理したい場合は、`Edit`→`Project Settings`→`Editor`から`Version Control`→`Mode`を`Visible Meta Files`に変更し、`Asset Serialization`→`Mode`を`Force Text`に変更

## 注意
　Google Tango搭載端末以外でRunすると`.apk`はインストールされますが、起動時にエラーが起きて強制終了します。