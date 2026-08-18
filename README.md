# 中指薙刀式（薙刀式に中指同時シフトを追加）

[薙刀式](https://oookaworks.seesaa.net/article/456099128.html#gsc.tab=0)を中指シフトでも打てるようにしたバージョンです。[v18（トップ版）](https://oookaworks.seesaa.net/article/521080503.html#gsc.tab=0)がベースになっています。

薙刀式の定義は基本的にそのまま内包しているので、元の薙刀式のままでも打てます。腱鞘炎の軽減や高速化のために中指シフトを併用できるようにしたバージョンになります。

## 打ち方

> [!Note]
> ドキュメントは現在整備中なので、詳しくはJSONなどの定義ファイルを確認してください。<br>
> [解説記事](https://nanagi.hatenablog.com/entry/2026/08/18/000334)も参考にしてください。

シフト面を打つ際、スペースの代わりに `D`・`K` との同時押しが使えます。

ただし例外として、
- 「や/ゆ/よ」は「C」との同時押し
- 「に」= `D + F`
- 「の」 = `J + K`
です。

中指同時シフトだけでなく、スペース (SandS) も併せて使うことができますので、打ち方は選ぶことができます。

## 設定ファイル

- やまぶきR（Windows）: [薙刀式v18_中指シフト.yab](https://github.com/ffunatsu/nanagi/blob/main/%E8%96%99%E5%88%80%E5%BC%8Fv18_%E4%B8%AD%E6%8C%87%E3%82%B7%E3%83%95%E3%83%88.yab) [^1]
- Karabiner-Elements（Mac）: [薙刀式v18_中指シフト.karabiner.json](https://github.com/ffunatsu/nanagi/blob/main/%E8%96%99%E5%88%80%E5%BC%8Fv18_%E4%B8%AD%E6%8C%87%E3%82%B7%E3%83%95%E3%83%88.karabiner.json)
- [obsidian-hechima](https://github.com/msonrm/obsidian-hechima) （Win/Mac/Linux/iOS/Android/ChromeOS）: [薙刀式v18_中指シフト.hechima.json](https://github.com/ffunatsu/nanagi/blob/main/%E8%96%99%E5%88%80%E5%BC%8Fv18_%E4%B8%AD%E6%8C%87%E3%82%B7%E3%83%95%E3%83%88.hechima.json)

## Hachiku-naka（Windows用）

https://github.com/ffunatsu/Hachiku-naka

Windowsでは、やまぶきR版 (.yab) に加えて↑のHachiku版も使えます。
こちらのほうが拗音拡張などで3打同時押しできるので薙刀式の定義により近いですが、中指同時シフトの定義と同時押し判定のアルゴリズムの相性のために、高速打鍵時に化ける文字が多く、化けるのが嫌であればやまぶきR版 (.yab) の利用をおすすめします。

## Benkei_naka (Mac用)

https://github.com/ffunatsu/Benkei_naka

Macでは、Karabiner-Elements版に加えて↑のBenkei版もあります。

Karabiner-Elements版との違いは、スペースキー（SandS）の連続シフトがサポートされているか否かで、中指シフトを併用している場合はさほど違いはないと思います。（文字の化けはKarabiner-Elements版のほうが少なく、IMEとの連動もそちらが安定しています。）

## その他メモ

- やまぶきR用の [`.yab`](https://github.com/ffunatsu/nanagi/blob/main/%E8%96%99%E5%88%80%E5%BC%8Fv18_%E4%B8%AD%E6%8C%87%E3%82%B7%E3%83%95%E3%83%88.yab) は、**UTF-16LEかShift-JISで保存しないと動作しません**。
- Karabiner-Elements版（ [`.karabiner.json`](https://github.com/ffunatsu/nanagi/blob/main/%E8%96%99%E5%88%80%E5%BC%8Fv18_%E4%B8%AD%E6%8C%87%E3%82%B7%E3%83%95%E3%83%88.karabiner.json) ）では、スペースキーの連続シフトが使えませんが、中指シフトを併用すれば大きな弊害はないと思います。
  - 一応 [Benkei](https://github.com/ffunatsu/Benkei) を中指薙刀式にフォークすることを検討していますが、未定です。
- HachikuとBenkeiは、固有名詞の登録など、様々な薙刀式特有の設定が可能です。編集レイヤーなどが使いたい場合はそちらを使ってください。

## License

このリポジトリ上の配布物については、CC0 とします。

ただし、[Hachiku-naka](https://github.com/ffunatsu/Hachiku-naka)と[Benkei_naka](https://github.com/ffunatsu/Benkei_naka)についてはライセンスが全く異なるため、各リポジトリを確認してください。

[^1]: やまぶきRでは通常キーの3打同時押しが使えないので、濁音拗音拡張は濁音キーの代わりに左親指シフトキー、半濁音拗音拡張は半濁音キーの代わりに右親指シフトキーとの同時押しに変化しています。
