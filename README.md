# 中指薙刀式（薙刀式 中指シフト化版）

薙刀式を中指シフトでも打てるようにしたバージョンです。v18 トップ版がベースになっています。

薙刀式の定義は基本的にそのまま内包しているので、元の薙刀式のままでも打てます。腱鞘炎の軽減や高速化のために中指シフトを併用できるようにしたバージョンになります。

ドキュメントは現在整備中なので、詳しくはJSONなどの定義ファイルを確認してください。

（基本的には、スペースの代わりにD/Kとの同時押しが使えます。「や/ゆ/よ」は「C」との同時押し、「に」= `D + F`、「の」 = `J + K` です。）

## Hachiku-naka（Windows用）

https://github.com/ffunatsu/Hachiku-naka

Windowsでは、やまぶきR版 (.yab) に加えて↑のHachiku版も使えます。
こちらのほうが拗音拡張などで3打同時押しできるので薙刀式の定義により近いですが、中指同時シフトの定義と同時押し判定のアルゴリズムの相性のために、高速打鍵時に化ける文字が多く、化けるのが嫌であればやまぶきR版 (.yab) の利用をおすすめします。

## Benkei_naka (Mac用)

https://github.com/ffunatsu/Benkei_naka

Macでは、Karabiner-Elements版に加えて↑のBenkei版もあります。

Karabiner-Elements版との違いは、スペースキー（SandS）の連続シフトがサポートされているか否かで、中指シフトを併用している場合はさほど違いはないと思います。（文字の化けはKarabiner-Elements版のほうが少なく、IMEとの連動もそちらが安定しています。）

## その他メモ

- `.hechima.json` は [obsidian-hechima](https://github.com/msonrm/obsidian-hechima) 用です。
- Karabiner-Elements版（ `.karabiner.json` ）では、スペースキーの連続シフトが使えませんが、中指シフトを併用すれば大きな弊害はないと思います。
  - 一応 [Benkei](https://github.com/ffunatsu/Benkei) を中指薙刀式にフォークすることを検討していますが、未定です。
- HachikuとBenkeiは、固有名詞の登録など、様々な薙刀式特有の設定が可能です。編集レイヤーなどが使いたい場合はそちらを使ってください。
- やまぶきR用の .yab は、UTF-16LEかShift-JISで保存しないと動作しません。

## License

このリポジトリ上の配布物については、CC0 とします。

ただし、[Hachiku-naka](https://github.com/ffunatsu/Hachiku-naka)と[Benkei_naka](https://github.com/ffunatsu/Benkei_naka)についてはライセンスが全く異なるため、各リポジトリを確認してください。