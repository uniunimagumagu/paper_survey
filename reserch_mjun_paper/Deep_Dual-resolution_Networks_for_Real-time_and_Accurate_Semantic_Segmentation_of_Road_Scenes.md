## Deep_Dual-resolution_Networks_for_Real-time_and_Accurate_Semantic_Segmentation_of_Road_Scenes

## Abstractの理解
CNNの改良っぽい。
CNNは畳み込みによってダウンサンプリングしている。セグメンテーションタスクはアップサンプリングとかする。
アップ、ダウンサンプリングにおいて有効性があるらしい。
CNNのアップサンプリングを使用するかは課題による。
本研究ではフーリエアップの設計について述べている。
そもそも、従来のCNNは空間アップサンプリング演算子を使用しているらしくそれが局所的な画素に影響受けるからだめって話。
じゃあ空間アップサンプリング演算子ってなに？？
→RCNN（逆畳み込み）、二アレストネイバ、バイリニア補完などのこと。こいつらは局所的すぎるからアップサンプルして復元したいとき大域性がない。セマセグとかで問題だよね。
そこでフーリエアップを提案している。
そもそも従来の画素中心のサンプリングは局所的で、大域的な手法としてフーリエ領域での変換がある。けどこれはアップサンプリングが難しかったが本研究ではフーリエアップを提案している。
# 議論すべき点
なし。
## 感想
すご。うちのセマセグで使えるのかな？？