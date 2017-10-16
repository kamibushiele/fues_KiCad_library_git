# これまで作ってきたKiCadライブラリ
## 構成
    +-library-(コンポーネントライブラリ)
    |   +-*.lib
    |   +-*.dcm
    |
    +-modules
        +-3Dmodels
        |   +-*(3Dモデルフォルダ)
        |   |   +-*.wrl
        |   |
        |   +-...
        |
        +-*.pertty(フットプリント)
        +-...
## 導入
### まずは
適当な場所にクローンしてくる
### コンポーネントライブラリの追加
リポジトリの`/library`以下をKiCadのコンポーネントライブラリに追加

### フットプリント用環境変数の追加
名前:`KIFUESMOD`

パス:`[リポジトリのパス]/modules`

### フットプリントライブラリの追加
__%appdata%\kicad__

にある

__fp-lib-table__

に以下を追加

      (lib (name fues-Battery_Holders.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-Battery_Holders.pretty)(options "")(descr ""))
      (lib (name fues-Buttons_Switches.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-Buttons_Switches.pretty)(options "")(descr ""))
      (lib (name fues-Buzzers_Beepers.pertty)(type KiCad)(uri ${KIFUESMOD}/fues-Buzzers_Beepers.pertty)(options "")(descr ""))
      (lib (name fues-capacitor.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-capacitor.pretty)(options "")(descr ""))
      (lib (name fues-connect.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-connect.pretty)(options "")(descr ""))
      (lib (name fues-display.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-display.pretty)(options "")(descr ""))
      (lib (name fues-Housings_DIP.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-Housings_DIP.pretty)(options "")(descr ""))
      (lib (name fues-IC_and_module.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-IC_and_module.pretty)(options "")(descr ""))
      (lib (name fues-LEDs.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-LEDs.pretty)(options "")(descr ""))
      (lib (name fues-mounting_hole.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-mounting_hole.pretty)(options "")(descr ""))
      (lib (name fues-PIC.pretty)(type KiCad)(uri ${KIFUESMOD}/fues-PIC.pretty)(options "")(descr ""))
      (lib (name fues-Relays.pertty)(type KiCad)(uri ${KIFUESMOD}/fues-Relays.pertty)(options "")(descr ""))


