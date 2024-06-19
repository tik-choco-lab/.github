# 分散型メタバースProject
本プロジェクトの目的は、メタバースに必要なプロトコルを確立し、相互運用性を向上させることである。

中央集権的な課題である単一障害点のリスクや、運用費用の捻出に依存するビジネスモデルから脱却し、
メタバースをより持続可能にするため、分散型ネットワークを採用する。

ユーザーは裏で動いているP2P技術を意識することなく、自動的に最適化されたシステムを利用できるようにする。
また、多くのメタバースプラットフォームが乱立する現状において、
統一的なプロトコルの確立を通じて相互運用性を促進する。

## miniverse
- https://github.com/DecentralizedMetaverse/miniverse
- 大学のオープンキャンパスで使用することを想定して作成したメタバース
- クライアントサーバー型であるが、だれでもサーバーを立てて実行できることから、ある種の分散型メタバースともいえるのでは？
- ワールド内のObject等は手打ちで指定する　アバターはVRMが使用できる
## location-sync
- https://github.com/DecentralizedMetaverse/location-sync
- ピュア型P2Pで仮想空間内のユーザー座標に基づいて、接続先を最適化するアルゴリズムの開発を行った。
- P2Pでの座標同期のシミュレーションプログラムである
## decentralized-metaverse-unity
- https://github.com/DecentralizedMetaverse/decentralized-metaverse-unity
- miniverseをベースとして分散型に改造することを目指していたたProjectだが、一から作り直した方が早いと考え、途中でfogverseとして作ることにした
## fogverse
- https://github.com/DecentralizedMetaverse/fogverse
- WebRTCを導入し、P2Pでのリアルタイム通信を実現
  - 複雑性を下げるために、MistNetを開発
- IPFSを導入したコンテンツ管理を実現
## MistNet
- https://github.com/DecentralizedMetaverse/mistnet
- fogverseにあったリアルタイム通信を分離させ、より広範囲のプロジェクトで適用可能にした。
- WebRTCを導入し、接続先最適化アルゴリズムを新たに導入している
## wuyu-protocol
- https://github.com/DecentralizedMetaverse/wuyu-protocol
- fogverseにあったコンテンツ管理を分離することを当初目指していたが、後々、相互運用性を向上させることの重要性に気づき開発を中断
## mistlib
- https://github.com/DecentralizedMetaverse/mistlib
- 相互運用性を向上させることを目的として、Unityからの脱却を行った
- メタバースにおける、リアルタイム通信とコンテンツ管理を提供する
- 現在、コンテンツ管理が70%ぐらいできている状態

# 分散型元宇宙项目
本项目的目的是确立元宇宙所需的协议，并通过提高互操作性来实现这一目标。

为了实现可持续的元宇宙，我们旨在采用分散型网络，摆脱集中式系统带来的单点故障风险和依赖运营费用的商业模式。

用户在使用系统时无需意识到后台运行的P2P技术，系统将自动进行优化，提供最佳体验。
同时，在目前众多元宇宙平台并存的情况下，我们也致力于通过确立统一的协议来促进互操作性。
