## 研究
### MC_Switching_MPI
- 富岳でマルチコンパートメントモデル用のシミュレータを高効率でシミュレーションする
  - ~ 2022/11/30：Switching法の導入
    - [ ] 過去の研究データ（）をもとに，MPI版の雛形となるPKJをGPUで動作するシミュレータ（PKJ_Switching_GPU）を作成
    - [ ] 全体的なリファクタリングを行う（無駄な変数などの修正）
    - [ ] BE，CNm，RK4，RKCが適切に動くことを確認する
    - [ ] 以下を見直し，適切な高速化を行う
      - [ ] SWC形式
      - [ ] CRS作成部分の
      - [ ] ガウスの消去法（不必要?）
      - [ ] 無駄なメモリ確保の是正
      - [ ] CG法の見直し（ガウスの消去法のほうがよい？？？）
      - [ ] CNをBEで簡易的に実装
    - [ ] Switching法の導入
    - [ ] PKJモデルを最新版に更新
    - [ ] ここまでできたらご褒美
  - ~ 2023/12/15：富岳での実行とさらなる効率化
    - [ ] PKJ_Switching_GPUをCPU版に**徐々に**以降（バグがでないことが大前提，少しずつ変更）
    - [ ] MPIへの変更と富岳での実行
    - [ ] JSONファイルへの対応
    - [ ] 調査した文献に基づいてGPU及びMPI版を調整
  - ~ 2023/12/30
    - [ ]

### SCA1
  - ~ 2023/12/15
    - [ ] GrC，GoC，PKJのモデルを見直す
      - [ ] GrC_Switching_MPIの作成
        - [ ] GPU版の再作成
        - [ ] CPUへの以降
        - [ ] MPI化
      - [ ] GoC_Switching_MPIの作成
        - [ ] GPU版の再作成
        - [ ] CPUへの以降
        - [ ] MPI化
    - [ ] ネットワークモデルを見直す
      - [ ] シナプス結合の効率の良い作り方
  - ~ 2023/12/30
    - [ ] Stellate，Basket，DCNを入れた小脳MCモデルを作成
      - [ ] Stellate cellのMPIモデルを作成
        - [ ] GPU版の再作成
        - [ ] CPUへの以降
        - [ ] MPI化
      - [ ] Basket cellのMPIモデルを作成
        - [ ] GPU版の再作成
        - [ ] CPUへの以降
        - [ ] MPI化
      - [ ] DCNのMPIのモデルを作成
        - [ ] GPU版の再作成
        - [ ] CPUへの以降
        - [ ] MPI化
      - [ ] ネットワークモデルの作成
    - [ ] 上記モデルで同期は作れるかを確認
      - [ ] IOの導入?

## 論文・本
- MCMシミュレーション関連
  - ~ 2023/11/30
    - [ ] SONATA
    - [ ] CoreNEURON
    - [ ] Scaffold Model
    - [ ] Arbor
    - [ ] NEURON
    - [ ] NEST
    - [ ] Brian
    - [ ] GENESIS
  - ~ 2023/12/15
    - [ ] MOOSE
    - [ ] Xolotl
    - [ ] Arbor
    - [ ] neuroConstruct
    - [ ] PyNN
    - [ ] NetPyNE
    - [ ] Open Source Brain
    - [ ] BMTK
    - [ ] 他の数値計算法の文献調査

- ニューロン形状の自動生成関連
  - ~ 2023/11/30
    - [ ] Computer generation and quantitative morphometric analysis of virtual neurons（次を決める）

  - ~ 2023/12/15

## 教科書 
### 読んだらListStudy_and_Seminarを更新
  - [ ] ゼロから作るDeep Learning 1（~2023/11/25）
  - [ ] One Point　推定と検定，鷲尾泰俊（~2023/11/30）
  - [ ] 入門統計学 -検定から多変量解析・実験計画法まで-，栗原伸一（~2023/12/15）
### 次の候補
  - [ ] 道具としてのベイズ統計
  - [ ] 数値計算の常識
  - [ ] スパコンプログラミング
  - [ ] CUDA Professional Programing
  - [ ] 常微分方程式の数値解法1










