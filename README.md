# WSL2Ubuntuja-tarFiles
WSL2環境で構築された日本語化されたUbuntu-24.04LTSのtarファイルです  
## 環境
・Windows11Home 23H2 (ライセンス認証済み)  
・64 ビット オペレーティング システム x64 ベース プロセッサ  

## tarファイルのダウンロード  
まず日本語Ubuntuのtarファイルをダウンロードします  
このURLにアクセスしてください  
`` https://mega.nz/folder/XbBwXS7L#HkI-j1t4fLb8GZNkil9RDg ``  
そして、ubuntucui.tar(CUIのみ)とubuntuxfce.tar(XFCE4デスクトップ環境)等から選んで、  
ファイルをダウンロードしてきてください  

## WSL2のインストール  
WSL2をインストールしないとWindowsにUbuntuをインストールする事はできません！  
なのでWSL2をインストールしていきましょう！  
まず、管理者権限のPowerShellで、下記のコマンドを実行してください  
`` Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux ``   
そしたら、Windowsを再起動しましょう  
  
## Ubuntuのインストール
Ubuntuをインストールしていきましょう  
WSL2をインストールしていない方は前のステップでインストールしてきてください   
WSL2をインストールしてきたら、まず以下のコマンドをcmdで実行してください  
`` wsl --update ``   
実行したら、cmdでtarファイルをダウンロードしたフォルダに移動して、以下コマンドを実行してください  
`` wsl --export Ubuntu-24.04 [ダウンロードしたファイル名] ``  
コマンドを実行し終わったら、コマンドプロンプトを再起動しましょう  
すると、起動メニューに「Ubuntu24.04LTS」というのがあるので、選択しましょう  
  
![image](https://github.com/Kawaharu869/WSL2Ubuntuja-tarFiles/assets/116153360/8096f7db-5100-4802-a220-a9dc1828dafc)  

これで、インストールは完了です！  
## デスクトップ環境の起動方法
Ubuntuのtarファイルでxfce4等のデスクトップ環境を選択した方へ向けてですが...  
Windows11のほうに標準で入っている「リモートデスクトップ接続」を使用します  
XRDPのIDは「localhost:3390」になります。  
良いWSL2Ubuntuライフを!
