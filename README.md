# Nature Remo BLE マクロコレクション

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/amanao/nature-remo-ble-macros.svg?style=social&label=Star)](https://github.com/amanao/nature-remo-ble-macros)
[![GitHub forks](https://img.shields.io/github/forks/amanao/nature-remo-ble-macros.svg?style=social&label=Fork)](https://github.com/amanao/nature-remo-ble-macros)

Nature Remo の BLE マクロ機能を使用して、様々な BLE デバイスを制御するためのマクロファイル集です。

## XML フォーマット
```xml
<macro name="マクロ名" icon="PLAY">
   <assert-service description="Ensure サービスUUID service" uuid="サービスUUID">
      <assert-characteristic description="Ensure キャラクタリスティックUUID characteristic" uuid="キャラクタリスティックUUID">
         <property name="WRITE" requirement="MANDATORY"/>
      </assert-characteristic>
   </assert-service>
   <write description="Write 0x値 to キャラクタリスティックUUID" characteristic-uuid="キャラクタリスティックUUID" service-uuid="サービスUUID" value="送信する値（16進数）" type="WRITE_COMMAND"/>
</macro>
```

## 参考資料
- [Nature Remo の BLE マクロ機能を使ってみよう！](https://engineering.nature.global/entry/ble-macro-control-beta)
- [Nature Developer Community (Discord)](https://discord.gg/3Ep57Muuuc)


## ライセンス
MIT License
