# wp-ja
- IOTAのホワイトペーパーの日本語訳のリポジトリ.
- 原著は[こちら](https://assets.ctfassets.net/r1dr6vzfxhev/2t4uxvsIqk0EUau6g2sw0g/45eae33637ca92f85dd9f4a3a218e1ec/iota1_4_3.pdf)
- 内容はBlockchainとはまた違うアイディアで(DAGを使って)DLTを考案したのでその大まかな理論的説明.
- 実際の実装は安全策がとられた(コーディネーターという安全弁が付与された)実装になっている.
- 2019年現在コンセンサスアルゴリズムはMCMCによるランダムウォークと累積荷重とコーディネータによってもたらされているが, コーディネータの排除手法である[coodicide](https://coordicide.iota.org)で提案された投票者モデルを応用したShimmerが提案され, 累積荷重を廃止し, Shimmerを中心とした多数のモジュールによってコンセンサスアルゴリズムを構築していくことになった.

### 簡単な特徴
- ブロック無し.
- 取引手数料無料.
- 自分より前の2つのトランザクションに矛盾がないか確認し, 承認するだけが必須ルール.
- あとはオプションのルールがあり, それに従うと後から来るトランザクションからの承認を受けやすくなる.
- そうすることで不特定多数の参加者がいてもナッシュ均衡が発生するようにする.(こちらの[論文](https://assets.ctfassets.net/r1dr6vzfxhev/2KfRHJKJW00kYcYkiuWaWk/342c5ccf54fd79993f2f33b9934a314f/Equilibria_in_the_Tangle.pdf))

### The Tangleに関するその他の学術論文
- https://www.iota.org/research/academic-papers

###  より詳しい説明
- https://coordicide.iota.org
- https://docs.iota.org
- [Assuring authenticity in the Tangle with signatures](https://blog.iota.org/assuring-authenticity-in-the-tangle-with-signatures-791897d7b998)
- [Running on the Tangle: a marathon of random walkers](https://blog.iota.org/running-on-the-tangle-a-marathon-of-random-walkers-99517d9b51a0)
- [Posets and Consensus](https://blog.iota.org/posets-and-consensus-fe4c034595ab)
- [Who’s In Who’s Out: a Rate Control Algorithm for the Tangle](https://blog.iota.org/whos-in-who-s-out-a-rate-control-algorithm-for-the-tangle-c7b5ecf85677)
- [The structure of the Tangle — Number of approvers](https://blog.iota.org/the-structure-of-the-tangle-number-of-approvers-326da2d7b3b0)
- [Mixing Time in The Tangle](https://blog.iota.org/mixing-time-in-the-tangle-439c2ba2ab31)
- [Coordinator. Part 4: An Open Source Coordinator](https://blog.iota.org/coordinator-part-4-an-open-source-coordinator-7d3804931058)
- [Coordinator. Part 3: Approaches to Coordicide](https://blog.iota.org/coordinator-part-3-approaches-to-coordicide-583fb82382bc)
- [Coordinator. Part 2: IOTA is a DAG, not a Blockchain](https://blog.iota.org/coordinator-part-2-iota-is-a-dag-not-a-blockchain-2df8ec85200f)
- [Coordinator. Part 1: The Path to Coordicide](https://blog.iota.org/coordinator-part-1-the-path-to-coordicide-ee4148a8db08)
- [Attack analysis - the simple parasite chain](https://blog.iota.org/attack-analysis-the-simple-parasite-chain-42a34bfeaf23)
- [Validity in the Tangle: The good, the bad, and the ugly](https://blog.iota.org/validity-in-the-tangle-the-good-the-bad-and-the-ugly-98bd3b53408a)
- [IOTA and Freedom](https://blog.iota.org/iota-and-freedom-bfc76770cd77)
- [On the Tangle, White Papers, Proofs, Airplanes, and Local Modifiers](https://blog.iota.org/on-the-tangle-white-papers-proofs-airplanes-and-local-modifiers-44683aff8fea)
- [Equilibria in the Tangle: let me try to explain… (part 2)](https://blog.iota.org/equilibria-in-the-tangle-let-me-try-to-explain-part-2-6dcc8e7c0ad8)
- [Equilibria in the Tangle: let me try to explain…](https://blog.iota.org/equilibria-in-the-tangle-let-me-try-to-explain-b22ad6f00c13)
- [Alpha: playing with randomness](https://blog.iota.org/alpha-d176d7601f1c)
- [Confirmation rates in the Tangle](https://blog.iota.org/confirmation-rates-in-the-tangle-186ef02878bb)
- [The Tangle: an illustrated introduction Part 5: Consensus, confirmation confidence, and the coordinator](https://blog.iota.org/the-tangle-an-illustrated-introduction-79f537b0a455)
- [The Tangle: an illustrated introduction Part 4: Approvers, balances, and double-spends](https://blog.iota.org/the-tangle-an-illustrated-introduction-1618d3e140ad)
- [The Tangle: an illustrated introduction Part 3: Cumulative weights and weighted random walks](https://blog.iota.org/the-tangle-an-illustrated-introduction-f359b8b2ec80)
- [The Tangle: an illustrated introduction Part 2: transaction rates, latency, and random walks](https://blog.iota.org/the-tangle-an-illustrated-introduction-c0a86f994445)
- [The Tangle: an Illustrated Introduction Part 1](https://blog.iota.org/the-tangle-an-illustrated-introduction-4d5eae6fe8d4)

### 発行年月日
- [The Tangle ver.1.4.3](https://github.com/solareenlo/iota-wp-jp/blob/master/wp-jp/iota1_4_3jp.pdf) (2018年4月30日)
- [The Tangle ver.1.4.2](https://github.com/solareenlo/iota-wp-jp/blob/master/wp-jp/iota1_4_2jp.pdf) (2018年2月9日)
- [The Tangle ver.1.4.1](https://github.com/solareenlo/iota-wp-jp/blob/master/wp-jp/iota1_4_1jp.pdf) (2017年11月27日)
- [The Tangle ver.1.4](https://github.com/solareenlo/iota-wp-jp/blob/master/wp-jp/iota1_4jp.pdf) (2017年10月25日)
- [The Tangle ver.1.3](https://github.com/solareenlo/iota-wp-jp/blob/master/wp-jp/iota1_3jp.pdf) (2017年10月1日)
- [The Tangle ver.1.2](https://github.com/solareenlo/iota-wp-jp/blob/master/wp-jp/iota1_2jp.pdf) (2017年8月22日)
- The Tangle ver.1.1 (2017年8月11日)
- The Tangle ver.0.6 (2016年4月3日)
