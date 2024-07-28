# 分散型メタバースProject
本プロジェクトの目的は、メタバースに必要なプロトコルを確立し、相互運用性を向上させることである。

中央集権的な課題である単一障害点のリスクや、運用費用の捻出に依存するビジネスモデルから脱却し、
メタバースをより持続可能にするため、分散型ネットワークを採用する。

ユーザーは裏で動いているP2P技術を意識することなく、自動的に最適化されたシステムを利用できるようにする。
また、多くのメタバースプラットフォームが乱立する現状において、
統一的なプロトコルの確立を通じて相互運用性を促進する。

# 分散型元宇宙项目
本项目的目的是确立元宇宙所需的协议，并通过提高互操作性来实现这一目标。

为了实现可持续的元宇宙，我们旨在采用分散型网络，摆脱集中式系统带来的单点故障风险和依赖运营费用的商业模式。

用户在使用系统时无需意识到后台运行的P2P技术，系统将自动进行优化，提供最佳体验。
同时，在目前众多元宇宙平台并存的情况下，我们也致力于通过确立统一的协议来促进互操作性。

# Why is a distributed network required?
## Centralized metaverse platforms are difficult to sustain
- Service rules can suddenly change; the service could be terminated by the organization
- High operational costs of cloud-based systems
- Business model dependency

## Toward Interoperability of Metaverse Real-Time Communication
**“Rough Consensus and Running Code”** is important and represents a history of internet standardization. 
It has been a key principle to realize interoperability. 
However, there are still few distributed network libraries which specialize in the metaverse and reach a high level of such interoperability.
To promote development, network libraries that anyone can easily use are an important option.

# Architecture

The metaverse consists of two layers:

1. Content Layer:
   - IPFS: The InterPlanetary File System (IPFS) is used for storing and sharing the content within the metaverse. It allows for distributed file storage and retrieval.

2. Realtime Layer:
   - WebRTC: Web Real-Time Communication (WebRTC) is utilized for the realtime layer of the metaverse. It enables communication and synchronization between users in the virtual environment.
   - Sync Object: Within the metaverse, objects can be synchronized in terms of their location and variables, allowing for interactions between users.

## Content Layer
![image](https://github.com/user-attachments/assets/93f811d8-f2b6-4af2-a3ce-76ff0886339f)

## MetaData
![image](https://github.com/user-attachments/assets/c8aca6b4-2e33-4cf5-b92f-d47c5045d669)

## Realtime Layer
Requirements for Real-Time Communication in the Metaverse
![image](https://github.com/user-attachments/assets/23e30b55-9839-47ba-80d9-f51a96b03218)


## WebRTC enables easier connections between different platforms
![image](https://github.com/user-attachments/assets/30c3ea8b-f949-4a01-96d1-53ed5b9c261f)


## Overlay Network and Distributed Signaling
- The message is sent directly or via other nodes
- With a decade of WebRTC, stable and reliable P2P connections are possible

![image](https://github.com/user-attachments/assets/33373ed1-01f0-44ea-a361-f0c0b6525d9e)

## Optimized using User Location in Virtual World
Exchange routing tables and user location with other nodes 

![image](https://github.com/user-attachments/assets/38252722-adfa-4156-a11f-59b05c2c3dbc)

## Secure P2P Authentication with Public Key Cryptography

- A user's public key also represents their user ID
- A message signed with a private key can be verified by the recipient using the public key, ensuring the identity of the sender

![image](https://github.com/user-attachments/assets/b51cca22-b1e0-4875-b063-38a82b97511a)


# 歴史 History
## 2022年 5月 miniverse
- https://github.com/DecentralizedMetaverse/miniverse
- 大学のオープンキャンパスで使用することを想定して作成したメタバース
- クライアントサーバー型であるが、だれでもサーバーを立てて実行できることから、ある種の分散型メタバースともいえるのでは？
- ワールド内のObject等は手打ちで指定する　アバターはVRMが使用できる
## 2022年 10月 location-sync
- https://github.com/DecentralizedMetaverse/location-sync
- ピュア型P2Pで仮想空間内のユーザー座標に基づいて、接続先を最適化するアルゴリズムの開発を行った。
- P2Pでの座標同期のシミュレーションプログラムである
- バーチャル学会で発表 https://doi.org/10.57460/vconf.2022.0_101
## 2022年 11月 decentralized-metaverse-unity
- https://github.com/DecentralizedMetaverse/decentralized-metaverse-unity
- miniverseをベースとして分散型に改造することを目指していたたProjectだが、一から作り直した方が早いと考え、途中でfogverseとして作ることにした
## 2023年 1月 fogverse

- https://github.com/DecentralizedMetaverse/fogverse
- WebRTCを導入し、P2Pでのリアルタイム通信を実現
  - 複雑性を下げるために、MistNetを開発
- IPFSを導入したコンテンツ管理を実現
- QRコードをスキャンしてワールドやコンテンツをやり取りできる
- IoTとも接続が可能であり、空間内から操作したりデータの取得ができる
- ICCE-Taiwan 2023で発表 https://doi.org/10.1109/ICCE-Taiwan58799.2023.10226934

![image](https://github.com/user-attachments/assets/e7f57458-69fb-4576-895e-de527c6540cb)


## 2024年 2月 MistNet
- https://github.com/DecentralizedMetaverse/mistnet
- Network library for the Metaverse and other network applications
- Focus on real-time communication
- Operates in a peer-to-peer (p2p) manner
- fogverseにあったリアルタイム通信を分離させ、より広範囲のプロジェクトで適用可能にした。
- WebRTCを導入し、接続先最適化アルゴリズムを新たに導入している

## 2024年 6月 wuyu-protocol
- https://github.com/DecentralizedMetaverse/wuyu-protocol
- fogverseにあったコンテンツ管理を分離することを当初目指していたが、後々、相互運用性を向上させることの重要性に気づき開発を中断

## 2024年 6月 mistlib ←今ここ
- https://github.com/DecentralizedMetaverse/mistlib
- 相互運用性を向上させることを目的として、Unityからの脱却を行った
- メタバースにおける、リアルタイム通信とコンテンツ管理を提供する
- 現在、コンテンツ管理が70%ぐらいできている状態
