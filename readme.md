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
        +-*.pretty(フットプリント)
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

      (lib (name fues-Battery_Holders)(type KiCad)(uri ${KIFUESMOD}/fues-Battery_Holders.pretty)(options "")(descr ""))
      (lib (name fues-Buttons_Switches)(type KiCad)(uri ${KIFUESMOD}/fues-Buttons_Switches.pretty)(options "")(descr ""))
      (lib (name fues-Buzzers_Beepers)(type KiCad)(uri ${KIFUESMOD}/fues-Buzzers_Beepers.pretty)(options "")(descr ""))
      (lib (name fues-capacitor)(type KiCad)(uri ${KIFUESMOD}/fues-capacitor.pretty)(options "")(descr ""))
      (lib (name fues-connect)(type KiCad)(uri ${KIFUESMOD}/fues-connect.pretty)(options "")(descr ""))
      (lib (name fues-display)(type KiCad)(uri ${KIFUESMOD}/fues-display.pretty)(options "")(descr ""))
      (lib (name fues-Housings_DIP)(type KiCad)(uri ${KIFUESMOD}/fues-Housings_DIP.pretty)(options "")(descr ""))
      (lib (name fues-Housings_SMD)(type KiCad)(uri ${KIFUESMOD}/fues-Housings_SMD.pretty)(options "")(descr ""))
      (lib (name fues-IC_and_module)(type KiCad)(uri ${KIFUESMOD}/fues-IC_and_module.pretty)(options "")(descr ""))
      (lib (name fues-LEDs)(type KiCad)(uri ${KIFUESMOD}/fues-LEDs.pretty)(options "")(descr ""))
      (lib (name fues-mounting_hole)(type KiCad)(uri ${KIFUESMOD}/fues-mounting_hole.pretty)(options "")(descr ""))
      (lib (name fues-Relays)(type KiCad)(uri ${KIFUESMOD}/fues-Relays.pretty)(options "")(descr ""))
