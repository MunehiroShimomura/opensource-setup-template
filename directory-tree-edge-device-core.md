aitrios-edge-device-build-linux/
│── t4-otoblite/
│  ├── yocto-bsp/		# 
│  	├── meta-xxx-boot
│  	├── meta-edge-device-core (s)
│── t4-refsys/
│  ├── yocto-bsp/		# 




edge-device-core-yocto/
  meta-edge-device-core-base
  meta-edge-device-core-nxp
  meta-edge-device-core-broadcom


or

aitrios-edge-device-build-linux/
│── t4
│  ├── yocto-bsp/		# 

or 

aitrios-edge-device-build/
 │── t4-otoblite/
 │── t4-refsys/
 │── t3p/
 │── t3pw/
 │── t5/


--------------------------------
edge-device-core/
├── src/			# ソースコード
│  ├── include/		# edge-device-core全体のinclude.ないかもしれない
│  ├── manager/		# manager格納用
│  │  ├── led/		# led manager
│  │  │  ├── include/	# 
│  │  │  ├── hal/		# 現状の構成はmanagerの下にhalがある？
│  │  ├── net/		# 必要な各manager。フォルダ構成はled同様
│  │  ├── xxx/
│  │  ├── yyy/
│  ├── app/			# Sysapp関連
│  │  ├── sysapp/		# 
│  │  ├── initapp/		# 
│  ├── senscord/		# subproject? or conan, vcpkgなど使った方が良いかも
│  ├── evp/			# subproject? or conan, vcpkgなど使った方が良いかも  クロスコンパイル対応してほしい cmake?
├── external/
│  ├── wamr/		# subproject? or conan, vcpkgなど使った方が良い？→ cont backするならsubmoduleがやりやすい？
│  ├── ...			# 
├── build/                   # ビルド用script
│   ├── debian		# Rasp-pi向け。debパッケージ生成まで
├── doc/			# ドキュメント（仕様書、APIリファレンスなど）
├── tool/			# 開発やビルドに必要なツールなど
├── script/			# インストールで必要なscript等あれば
├── test/			# テストに必要な一式。テストベンチ、テストデータ、テストシナリオ等
├── Makefile			# make master (CmakeつかうならCmakeLists.txt等)
├── Makefile.config		# make master (CmakeつかうならCmakeLists.txt等)
├── README.md
├── LICENSE			# 対象物のライセンスの明示
├── CONTRIBUTING.md		# コントリビューションのガイド
├── CODE_OF_CONDUCT.md	# 行動規範・コントリビューション権利の扱い宣言
├── SECURITY.md 		# セキュリティに対する行動規範・ガイド
├── PULL_REQUEST_TEMPLATE.md	# Pull Req時のテンプレート  .githubしたかも
├── ISSUE_TEMPLATE.md　　　　#.githubしたかも
├── CODEOWNERS
├── CHANGES.md





edge-device-core.deb
  - libwamr.so
  - libsenscord.so
  - libevp.so
  - libesf.so
  - sysapp

json.deb
  - libjson.so

jpeg.deb
  - libjpeg.so

