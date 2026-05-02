NoMosaic for Looser Maker

概要
----
ルーザーメーカー用のBepInEx 6 IL2CPPプラグインです。
キャラ配下の既知モザイクオブジェクトだけを無効化します。
全フィールドのRendererを総当たりしないため、常駐負荷を抑えています。

導入
----
1. ゲームフォルダにBepInEx 6 IL2CPPを導入してください。
   同梱の BepInEx-Unity.IL2CPP-win-x64-6.0.0-be.755+3fab71a.zip を展開します。
2. このzip内の BepInEx フォルダをゲームフォルダへ上書きコピーしてください。
3. ゲームを起動します。

操作
----
F8: NoMosaic 有効/無効切り替え
F9: 設定再読み込み + 手動スキャン

設定
----
BepInEx/config/local.nomosaic.loosermaker.cfg

RootNames:
  モザイクを探すキャラルート名です。
  現在は Player,Man を対象にしています。

RelativeTargetPaths:
  キャラルートから見たモザイク子オブジェクトの相対パスです。

TargetNames:
  相対パスで見つからない場合に、キャラルート配下だけで探す名前です。

現在の対象
----------
Player/ModelRoot/Model/nazury/Armature/Hips/mosaic
Player/ModelRoot/Model/nazury/Armature/Hips/mosaic2
Man/Mesh/モザイク

メモ
----
実フィールドで別キャラ名や別階層のモザイクが残る場合は、
RootNames や RelativeTargetPaths に対象を追加してください。
