# my-qmk-configure

## キーマップ更新手順

### AnnePro2

1. [QMK Configurator](https://config.qmk.fm/#/annepro2/c18/LAYOUT_60_ansi)でキーマップを作成し、GUI 上でコンパイル+ファームウェアの DL をする。
1. ESC を押しながら AnnePro2 を PC に接続する
1. AnnePro2 Tools を取得
   https://github.com/OpenAnnePro/AnnePro2-Tools
1. [AnnePro2](https://github.com/OpenAnnePro/AnnePro2-Tools#readme)の Readme を参考にキーマップを反映する。
   1. rust をインストールする。
   1. AnnePro2 Tools を`cargo build --release`でビルドする。
   1. `./target/release/annepro2_tools keymap.bin`でキーボードにキーマップを書き込む。
