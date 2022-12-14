# Linuxの概要

## サーバとは
### サーバ(server)とは **「サービスを提供する役割のコンピュータ」** のこと
* Webサービスを提供するWebサーバやメールサービスを提供するメールサーバ等、種類は多岐に渡る  
* あくまでもサービスを提供する役割のことをサーバと呼び、**サーバという名前の機械があるわけではない**  

* サービスを提供する「サーバ」に対し、サービスを受け取る側のことを「**クライアント**」という\
![md1]("Pictures\Screenshotzs\md1.png")
<!--
図を入れる
-->

<br>
<br>

### サーバに必要な条件
サーバは常時起動し多数のアクセスに対応するため、高いスペックを求められることが多い。\
ノートPCでもサーバの役割を担うことは可能だが、ノートPCはサーバ用として使われる前提での設計がされていない為、物理的、電気的な設計に余裕がなく連続稼働に耐えられない。\
また、単純にスペック不足によりサーバーとして最低限の動作すら不可能なケースもある。
\
<br>

下記3点のように、サーバとしての利用を想定されて作られている機械がある。


* タワー型サーバ  
  -小規模なシステムに用いられることが多い  
  据え置き型で、購入後すぐに使用することができる  
  専用のサーバーラックが不要となるため、導入コストを抑えることができる
* ラックマウント型サーバ  
  -中規模から大規模なシステムに用いられることが多い  
  サーバーや関連機器などが専用のラックに格納されるため、重要なデータを厳重に管理できたり、保守やメンテナンスが容易になったりすることが特徴
* ブレードサーバ  
  -大規模なシステムに用いられることが多い  
  サーバーブレードという薄いサーバを専用のラックに差し込んで使うサーバのこと  
  サーバブレードを差し込むだけで配線作業をせずに増設できるため、作業工数やサーバを置くスペースを削減することができる

  <!--ここに各サーバのイラスト入れる検討中→入れてほしいです！！！→画像探し中
  -->
<br>
<br>

## OSとは
### OS(Operating System)とはコンピュータの基本的な処理を担当するソフトウェアのこと  

<br>

### コンピュータの基本的な処理とは
* マウスやキーボード、ディスプレイなどの入出力処理
* アプリケーションの実行
* CPUやメモリ、HDDやSSDの制御  
<br>

代表的なOSの例としてWindows,MacOS,iOSなどが挙げられる。

<br>


<!---
ハードウェアとソフトウェアの違いの前にまず説明したほうがいい
--->
### ハードウェアとソフトウェアの違い
**ハードウェア**  
目に見える機器全般を指し、物理的実体を持っている。  
ハードウェア単体では機能せず、ソフトウェアが存在して初めて動作する特徴を持つ。  
キーボードやマウス、メモリやHDD、CPUなどが該当する

**ソフトウェア**  
コンピュータを動作させるための手順や命令を、コンピュータが理解できるプログラミング言語で記述されたものを指す。  
ソフトウェアは物理的実体を持たず、目で見たり触れたりはできない。  
OSというソフトウェアがなければPCというハードウェアが動作しないように、非常に高い重要性をもつ。
ソフトウェアの中でも、システムソフトウェアとアプリケーションソフトウェアの2種に分かれることが多い。

* システムソフトウェア  
  基本的制御や管理を行う。
  OSなどのシステムが含まれる。  

* アプリケーションソフトウェア  
  資料作成や分析など**特定の用途や目的ため**に使われるソフトウェア。
  表計算ソフトやメールソフトなどが含まれる。

<br>

## OSの種類
OSにはデスクトップ用・サーバ用・モバイル用があり、その種類は多岐にわたる。

![OS比較表]("C:\Users\minami.hiruma\Desktop\14_training_materials_15days\day1\1.linux_overview(server)\os_diagram.png")

<!--
Excelで作ったOS比較のリストを挿入予定,格納先のパスは上記の通り
-->

<br>

## Linuxとは
### Linuxとは主にサーバに用いられるOSの一種
Linuxには数多くの種類が存在し、それら1つ1つのことを「Linuxディストリビューション」と呼ぶ。  
<!--
「総じて」は少し違いますね。
-->
その中でもDebianから派生した **Debian系統**とRed Hat Enterprise Linuxから派生した **Red Hat系統**等の分類がある。

代表的なディストリビューションは以下の4つ

<br>

### Debian
* ボランティアの技術者により開発・運営が行われている無料のOS
* ディストリビューションのシェア率は第2位

<br>

### Ubuntu
*ディストリビューションのシェア率は世界1位
* 企業に技術的・金銭的支援を受けている無料のOS
* Debian系だが、Debianよりも先進的でリリースが非常に速い

<br>

### Red Hat Enterprise Linux(RHEL)
* Red Hat社が開発している商用向けのディストリビューション(有料)
* 有料のディストリビューションでは最もよく使われている
* 手厚い商用サポートが受けられることが特徴

<br>

### CentOS
* 一言でいうと「RHELの無料版」
* 基本的にはRHELと同じだが、商用のサポートはない  
  また、RHELでは利用できるがCentOSでは利用できないアプリなどもある

<br>

![distribution]("C:\Users\minami.hiruma\Desktop\training_materials_15days\day1\1_linux_overview(server)\distribution_diagram.png")

<!--Excelで作成したディストリビューションの比較リストを挿入予定,格納先のパスは上記-->