# 1.  背景

ABC予想は，およそ30年前に定式化されたばかりの予想ではあるが，数論における最も重要な予想のひとつである．複数の定式化が存在するが，そのうちには際立った有限性定理やその他の結果に繋がる定式化や，或いはこの予想の証明にあたって頑健な系統的アプローチを与えうる定式化がある．この予想は，任意の正整数ペア（AとB）とその和（C）の素因数を，これらの数たちおよびその和と結び付ける具体的な不等式に関するものである．ABC予想には，より大きな数の体系（「数体」と呼ばれ，数論において常に現れる）における自然な拡張が存在する．

ここでは，自然数の場合を対象として，この予想の正確な主張とその帰結に関して議論・説明する．重要な応用も自然数の場合において述べる．ABC予想に現れるような，自然数の乗法的性質と加法的性質の相互作用は，やや繊細な問題である（例えば，pを素数としたとき，p + 12 の素因数分解について非自明なことは何も言えない）．この予想で現れる不等式には，制限の度合いを表現する補助的定数が含まれており，このことによって多くの条件下で際立った帰結をもたらす．以下で議論しよう．

ABC予想が重要なのは，その多くが定式化された当初には予想もされていなかった豊富な理論的帰結である．（この予想とそのもたらす結果の多くについては，代数体上での定式化に一般化することが不可欠である．）

1980年代半ばに定式化された時点から，ABC予想が Mordell 予想に対する effective な証明（「大きな種数」をもつ代数曲線の有理点の数を明示的にバウンドすること．単に有理点の数の有限性を示すより遥かに難しい；なお［effective でない］Mordell 予想は，このような点の集合が有限個しかないことを主張するものであり，Faltings よって1980年代に証明され，彼はこの成果によって Fields 賞を授与された）といった，他の未解決問題と深いつながりがあり，また時に等価であることは知られていた．Moderll 予想に対する明示的な解を導くためには，ABC不等式の定数を明示的に求めなければならない．

等価な定式化には「楕円曲線」を用いるものがある．楕円曲線とは，2変数3次方程式によって定義される曲線であり，数論における数多くの問題（特に，Fermat の最終定理を含む）に登場する．Lucien Szpiro は，楕円曲線の不変量に関してある不等式が成立することを予想した（Szpiro予想）．ABC予想が David Masser と Joseph Oesterle によって定式化されてから暫くしてのち，任意の代数体上での定式化に一般化すれば，AB C予想と Szpiro 予想とは等価であることが知られるところとなった（これは「Frey 曲線」と呼ばれる，Fermat の最終定理と楕円曲線とを関係づける際にも用いられるある特別なクラスの楕円曲線を用いて証明される）.

望月新一は Faltings のもとで 1992 年に Ph.D. を取得して以来，京都の 数理解析研究所 (RIMS) で研究をしている優れた数学者である．彼がこの問題を長期的な達成目標として，少しずつ彼の専門分野（数論幾何，特に遠アーベル幾何）において深い技術的進歩を積み上げていることは長きにわたって知られていた．［望月のアプローチにおいては，］Fermat の最終定理と同様，この予想に関して何らかの結果をもたらすためには，最初の定式化にあるような具体的な数同士の関係を直接取り扱うことはしない．かわりに，具体的な数を取り扱うのでは利用不可能なより強力な道具や操作を利用可能とするよう，ABC予想は代数幾何学におけるより精緻な理論的構築物に基づいて再定式化される．望月の目標は Szpiro 予想の証明だった．

2012年8月，望月は「宇宙際 Teichmüller 理論」と彼が呼ぶ理論によってこの問題を解決したと宣言した：彼はこの予想の証明で終わる，長いプレプリント群を公開した．望月は際立って優れた（そして，非常に注意深い）数学者であり，また彼のABC予想に対するアプローチ（楕円曲線に関する Szpiro 予想を経由するアプローチ）は，遠アーベル幾何学において彼自信がこれまでに編み上げてきた深い幾何学的・群論的理論の壮大な絵巻物に基づくものである．長い期間にわたって，この問題を解決するための道具の構築と適用に相当の労力を費してきたことに関して，彼は尊敬されて然るべきである．

望月の今現在の手法では，明示的な定数を得ることはできず，Mordell 予想の effective な証明にはならない．しかしいずれにせよ，この証明が正しいとすれば，様々な未解決の難問を解決するとともに Mordell 予想の新たな証明となる（この点はずっと昔に Noam Elkies が証明している），驚異的な成果だと言える．

専門家たちは，この証明が正しいか検証するのが非常に難しいということを直ちに理解した．証明が書かれた論文は，非常に多数の不慣れな用語や記法と具体例なしの定義の羅列が続く形式で書かれており，代数幾何学に関する十分な知識を持つ読者でさえもこの論文を読み進めようとするにあたり自分が進歩しているという感覚を持つことを困難にした．論文にはアナロジーやモチベーションを述べる数多くの注釈が存在するが，初めて読む多くの読者にとってはこれらの注釈の重要性や，アナロジーの意味を理解することは難しい．普通の論文に比べて「モチベーション」に関する議論が非常に多いことからすれば逆説的であるが，多くの読者はすぐに落胆するか或いは混乱してしまい，読むのを止めてしまった．論文本体を読む困難さに加え，望月はメールでの質問には意欲的に答えるとともに RIMS への直接の訪問者との議論には応ずるものの，この論文に関する出張や講演をしなかった．

今日に至るまで，彼の遠アーベル幾何に基づくABC予想の証明のアイデアを広め評価するためには多くの課題が残っている．代数幾何コミュニティに属する多くの人のやる気が削がれていることが状況を停滞させる要因となっている．この状況をここで説明する．

当初の宣言から3年が経過したとは言うものの，この時間のあいだ多数の代数幾何学者が論文の検証をしていたというわけではない．どちらかと言えば，多くの人が初期に挑戦してすぐにやる気を削がれてしまった（部分的には，新奇な記号，用語，考え方が余りに多過ぎたせいで）．サーベイ論文も数本書かれたが，私が話したことがあるほぼ全ての人が，もとの論文と同様，これらのサーベイから啓蒙を得るのは難しいと述べた．（なかには理解が進んだという人もいたが，多くはそうではないかった）

クレイ数学研究所とオックスフォード大学数学研究所は，重要な一歩を踏み出した．ABC予想に関連する代数幾何学の諸分野の専門家（宇宙際 Teichmüller 理論を検証してはいない）を集め，望月の研究に関するワークショップを開催したのである．目的は，専門家集団として，あまりにやる気を削がれて数学者個々人では成し遂げられなかった，大筋の理解を進めようとしたのである．主催者はこの集会の開催のために尋常でない労力を費したし，（CMIのスタッフも含め，）賞賛されるべきである．研究集会を開催するために十分な講演者を集めるのは難しかった．多くのベテランは講演したがらなかったし，また講演者の多くにとって望月の研究対象（例えば Frobenioids やエタール・テータ関数）は完全に新規なものだった．当然のことながら，講演者の多くは，自分の講演内容が最終的に全体の流れのどこに位置することになるのかしばしば理解できていなかった．狙いは，ひとりひとりの努力が組合わさることで，全体としての理解が進むのではないかということだった．

私はこのワークショップに参加した．参加者のうちには Alexander Beilinson, Gerd Faltings, Kiran Kedlaya, Minhyong Kim, Laurent Lafforgue, Florian Pop, Jakob Stix, Andrew Wiles, そして Shou-Wu Zhang といった，著名な代数幾何・遠アーベル幾何の研究者たちもいた．全参加者のリストは[ここ] (https://www.maths.nottingham.ac.uk/personal/ibf/files/symcor.iut.html)に公開されている．

証明の正しさを検証することは，このワークショップの目的ではなかった．私の（そして他の多くの参加者の）理解では，目的は代数幾何の様々な分野から集まった参加者が望月の研究全体の鍵となるアイデアに関する理解を深め，（特には）望月の論文を読もうとするにあたって多くの数学者が感じたやる気が削がれる感覚を緩和することだった．

望月の研究は深いアイデアに基づいて，それ自体は主流の代数幾何学の文脈に即している新しいツールを構築・分析し，ABC 予想に対する新たなアプローチ法を与えることだ．しかし，数学において，難しい証明の正しさを検証するには様々なレイヤーでの理解が必要であり，その最初のステップは，優れて新しい着想がどこにあるかのと，それがおおよそどのようにして結果としての主張をもたらすのかに関する明確な理解である．現状では望月の研究に関するそのような理解が（少なくとも代数幾何学の研究者の多くにとって納得のいくレベルでは）存在せず，論文で何がなされたのかが現在でも広く理解されていない主要因となっていた．このような「主たる着想の理解」について，ワークショップは確固たる進歩を成し遂げたといえ，その意味で有益なものだった．

ワークショップには，多くの人が望んでいた「アハ！体験」は存在しなかった．私は，週の後半にかけてたまった強いフラストレーションにもかかわらず，この Oxford でのワークショップに参加してよかったと思っている．多くの参加者は理論の部分部分や，主な課題がどこに存在するのかに関して理解を深められたが，宇宙際 Teichmüler 理論に関するエキスパートにはなれなかった（私の意見では，これはワークショップの目標ではなかったと思う）．ワークショップの発表のなかでは，様々な理論や中間的な結果が相互に深く関係し合う様子や，望月の様々な過去の結果が色々の部分に入り込んでくる様子が見られた．彼が注意深くかつパワフルな数学者であるというこれまでの記録も考えに入れれば，この研究は真剣に検証されるべきものであると言える．

「聴衆の」意見や期待に関する下記の記述は，（一般に宇宙際 Teichmüler 理論の専門家ではない代数幾何の専門家である）参加者たちと私が交わした会話に基いている．私の知る限りでは，このワークショップに関する期待や，この一週間で何が起こったかについての感想について，参加者の考えは一致しているようだ．この文書に書かれていることの不正確性は，究極的には私の責任である．修正があれば歓迎です（効率のため，このサイトのコメント機能を使ってください）．



# 2. 基本的な考え方の理解を遅らせたのは何か？

主たる考え方が広く理解されることの妨げになったのは，この論文の前提となっている研究が長い年月にわたる研究に基づいている点だろう．しかもこの長い年月のあいだ，どの部分が主定理の証明のみを理解するために最終的に必要となるのかわかっていなかった．これまで，主たる定理を導くための論理の流れがわかるような用語・記号の定義を用いた一貫した議論を与えるような「掃除」はなされていない．（最終的には）こうした掃除が必要だ．

望月は，代数体上のすべての楕円曲線に関する Szpiro 予想の証明（定数が代数体の次数と，$$ε$$のみに依存するもの）を目的としている．この予想からより具体的な結果（例えば ABC 予想，そして従って様々な有限性定理：モーデル予想，アフィン曲線の整数点に関する Siegel の定理，そして the finiteness of the set of elliptic curves over a fixed number field with good reduction outside a fixed finite set of places）への帰結は何十年も昔から知られており，彼の議論において一切登場しない．特に，このような具体的結果に関する議論によって望月の手法が正しいかどうか「試す」ことはできない．彼の全ての議論は Szpiro 予想の文脈でなされているからである（この文脈では，具体的な結果は一切関係しない）．

しかも，彼の手法は対象とする楕円曲線に関してある大域的・局所的性質を要求する（such as having split 30-torsion and split multiplicative reduction at all bad places）が，これらの性質は Frey 曲線は一般に満足せず，適切な次数をもつ基礎体の拡大において満足される．彼はこうした特殊例を用いつつ，こうした特殊例から一般の場合（任意の代数体！）に拡張可能な短いが賢い主張を抽出する — 定数を明示的に求められなくなるかわりに．したがって，彼の手法を有理数の集合のような小さな基礎体で直接適用することはできない；有理整数に関するもともとの不等式は，比較的大きな（しかし適切な）次数を持つ代数体における結果から従うのである．

時には他の先行する一般に不慣れな内容（Frobenioid や anabeliod）に関する論文への後方参照がなされ，数多くの新しい概念を理解する必要に迫られ，結果として無限退行するかのような印象が生み出される．これもまたやる気を削ぐ効果をもたらした．しばしば望月の議論は一般論から具体論へ進むという形をとるからである（論理としてはよいだろうが，新しい概念を学ぶ際には必ずしもよい順序とは言えない）．例えば，もし望月の理論における Frobenioid（この単語は「Frobenius」と「monoid」の合成語である)という重要な概念を理解しようとしたとき，モチベーションが彼の楕円曲線に関する Hodge-Arakelov 理論の研究から来ていることがわかるが，この結果として2つの（数学的なというよりは）心理的な障害にぶつかる：
1. Hodge-Arakelov 理論は最終的には使われない（代数的 小平-Spencer 理論を構築することが，関数体の場合に触発された望月の最初の狙いであったが，このアプローチは失敗した）．最終的には使われないとしたら，どれだけの時間をモチベーションを理解するためだけに非自明な理論の学習に費すべきなのだろうか？（もし費すとしたらだが）
2. Frobenioids の理論に関するほとんどの部分（望月の先行する2つの論文の内容）も，最終的には使われない（特殊例のみで十分である）が，最初に学ぼうとした読者は気付かないかもしれず，また全ての理論を理解しなければならないと（誤って）思うかもしれない．望月の Web ページに，究極的にはこの理論の殆どが使われないことを述べている短い注があるが，独学している人は気付かないかもしれない．例えこの注釈を発見し，これらの先行する論文のうち最終的に使われる重要な特殊例を取り扱った部分のみを読もうとしても，膨大な記号・用語や，前の方で述べられている結果が使用されているのを目にすることになる．こうして，「特殊例を理解するためだけでも結局のところ最も一般的な議論を理解するために最初から読まなければならないのではないか」という恐怖を（間違ってはいるものの）感じ，結局はやる気を失ってしまうかもしれない．

これは Grothendieck のエタール・コホモロジーを学ぶときのことを思い起こさせる．近年ではこの理論を一から直接的かつ（多かれ少なかれ）効率的なやりかたで構築し，重要な定理を証明していくようなよい本がいくつかある．Grothendieck の数分冊に渡る SGA4 における最初の定式化においては，非常に抽象的なトポスの一般理論を構築するために何百ページも割かれている．これは後の様々な一般化のための基礎となることを目指して書かれていた（そして後に実際に一般化された）．このような非常な一般性はしかし，エタール・コホモロジーのみを理解しようとするためには（任意の圏を理解するためにさえも）完全に不必要である．


# 3. 宇宙際 Teichmüler 理論 (IUT) とは何か？

I will build up to my impression of an approximate definition of IUT in stages. As motivation, the method of Mochizuki to settle Szpiro’s Conjecture (and hence ABC) is to encode the key arithmetic invariants of elliptic curves in that conjecture in terms of “symmetry” alone, without direct reference to elliptic curves. One aims to do the encoding in terms of group-theoretic data given by (arithmetic) fundamental groups of specific associated geometric objects that were the focus of Grothendieck’s anabelian conjectures on which Mochizuki had proved remarkable results earlier (going far beyond anything Grothendieck had dared to conjecture). The encoding mechanism is addressed in the appendix; it involves a lot of serious arguments in algebraic and non-archimedean geometry of an entirely conventional nature (using p-adic theta functions, line bundles, Kummer maps, and a Heisenberg-type subquotient of a fundamental group).

Mochizuki’s strategy seems to be that by recasting the entire problem for Szpiro’s Conjecture in terms of purely group-theoretic and “discrete” notions (i.e., freeing oneself from the specific context of algebro-geometric objects, and passing to structures tied up with group theory and category theory), one acquires the ability to apply new operations with no direct geometric interpretation. This is meant to lead to conclusions that cannot be perceived in terms of the original geometric framework.

To give a loose analogy, in Wiles’ solution of Fermat’s Last Theorem one hardly ever works directly with the Fermat equation, or even with the elliptic curve in terms of which Frey encoded a hypothetical counterexample. Instead, Wiles recast the problem in terms of a broader framework with deformation theory of Galois representations, opening the door to applying techniques and operations (from commutative algebra and Galois cohomology) which cannot be expressed directly in terms of elliptic curves. An analogy of more relevance to Mochizuki’s work is the fact that (in contrast with number fields) absolute Galois groups of p-adic fields admit (topological) automorphisms that do not arise from field-theoretic automorphisms, so replacing a field with its absolute Galois group gives rise to a new phenomenon (“exotic” automorphisms) that has no simple description in the language of fields.

To be more specific, the key new framework introduced by Mochizuki, called the theory of Frobenioids, is a hybrid of group-theoretic and sheaf-theoretic data that achieves a limited notion of the old dream of a “Frobenius morphism” for algebro-geometric structures in characteristic 0. The inspiration for how this is done apparently comes from Mochizuki’s earlier work on p-adic Teichmuller theory (hence the “Teichmuller” in “IUT”). To various geometric objects Mochizuki associates a “Frobenioid”, and then after some time he sets aside the original geometric setting and does work entirely in the context of Frobenioids. Coming back to analogues in the proof of FLT, Wiles threw away an elliptic curve after extracting from it a Galois representation and then worked throughout with Galois representations via notions which have no meaning in terms of the original elliptic curve.

The presence of structure akin to Frobenius morphisms and other operations of “non-geometric origin” with Frobenioids is somehow essential to getting non-trivial information from the encoding of arithmetic invariants of elliptic curves in terms of Frobenioids in a way I do not understand and was not clearly addressed at the Oxford workshop, though it seems to have been buried somewhere in the lectures of the final 2 days; to understand this point seems to be an essential step in recognizing where there is some deep contact between geometry and number theory in the method.

So in summary, IUT is, at least to first approximation, the study of operations on and refined constructions with Frobenioids in a manner that goes beyond what we can obtain from geometry yet can yield interesting consequences when applied to Frobenioid-theoretic encodings of number-theoretic invariants of elliptic curves. The “IU” part of “IUT” is of a more technical nature that appears to be irrelevant for the proof of Szpiro’s conjecture.

The upshot is that, as happens so often in work on difficult mathematical problems, one broadens the scope of the problem in order to get structure that is not easily expressible in terms of the original concrete setting. This can seem like a gamble, as the generalized problem/context could possibly break down even when the thing one wants to prove is true; e.g., in Wiles’ proof of FLT this arose via his aim to prove an isomorphism between a deformation ring and a Hecke ring, which was much stronger than needed for the desired result yet was also an essential extra generality for the success of the technique originally employed. (Later improvements of Wiles’ method had to get around this issue, strengthening the technique to succeed without proving a result quite as strong as an isomorphism but still sufficient for the desired final number-theoretic conclusion.)

One difference in format between the nature of Mochizuki’s approach to the Szpiro Conjecture and Wiles’ proof of FLT is that the latter gave striking partial results even if one limited it to initial special cases – say elliptic curves of prime discriminant – whereas the IUT method does not appear to admit special cases with which one might get a weaker but still interesting inequality by using less sophisticated tools (and for very conventional reasons it seems to be impossible to “look under the hood” at IUT by thinking in terms of the concrete consequences of the ABC Conjecture). Mochizuki was asked about precisely this issue during the first Skype session at the Oxford meeting and he said he isn’t aware of any such possibility, adding that his approach seems to be “all or nothing”: it gives the right inequality in a natural way, and by weakening the method it doesn’t seem to simply yield a weaker interesting inequality but rather doesn’t give anything.

Let us next turn to the meaning of “inter-universal.” There has been some attention given to Mochizuki’s discussion of “universes” in his work on IUT, suggesting that his proof of ABC (if correct) may rely in an essential way on the subtle set-theoretic issues surrounding large cardinals and Grothendieck’s axiom of universes, or entail needing a new foundation for mathematics. I will now explain why I believe this is wrong (but that the reason for Mochizuki’s considerations are nonetheless relevant for certain kinds of generalities).

The reason that Mochizuki gets involved with universes appears to be due to trying to formulate a completely general context for overcoming certain very thorny expository issues which underlie important parts of his work (roughly speaking: precisely what does one mean by a “reconstruction theorem” for geometric or field-theoretic data from a given profinite group, in a manner well-suited to making quantifiable estimates?) He has good reasons to want to do this, but a very general context seems not to be necessary if one takes the approach of understanding his proofs along the way (i.e., understanding all the steps!) and just aiming to develop enough for the proof of Szpiro’s Conjecture.

Grothendieck introduced universes in order to set up a rigorous theory of general topoi as a prelude to the development of etale cohomology in SGA4. But anyone who understands the proofs of the central theorems in etale cohomology knows very well that for the purposes of developing that subject the concept of “universe” is irrelevant. This is not a matter of allowing unrigorous arguments, but rather of understanding the core ideas in the proofs. Though Grothendieck based his work on a general theory of topoi rather than give proofs only in the special case of etale topoi of schemes, it doesn’t follow that one must do things that way (as is readily seen by reading any other serious book on etale cohomology, where universes are irrelevant and proofs are completely rigorous).

In other words, what is needed to create a rigorous “theory of everything” need not have anything to do with what is needed for the more limited aim of developing a “theory of something”. Mochizuki does speak of “change of universe” in a serious way in his 4th and final IUT paper (this being a primary reason for the word “inter-universal” in “IUT”, I believe). But that consideration of universes is due to seeking a very general framework for certain tasks, and does not appear to be necessary if one aims for an approach that is sufficient just to prove Szpiro’s Conjecture. For the purposes of setting up a general framework for IUT strong enough to support all manner of possible future developments without “reinventing the wheel”, the “inter-universal” considerations may be necessary, and someone at the Oxford workshop suggested model theory could provide a well-developed framework for such matters, but for applications in number theory (and in particular the ABC Conjecture) it appears to be irrelevant.

# 4. ワークショップで何があったか？

The schedule of talks of the workshop aimed to give an overview of the entire theory. The aim of all participants with whom I spoke was to try to identify where substantial contact occurs between the theory of heights for elliptic curves (an essential feature of Szpiro’s Conjecture) and Mochizuki’s past work in anabelian geometry, especially how such contact could occur in a way which one could see did provide insight in the direction of a result such as Szpiro’s conjecture (rather than just  yield non-trivial new results on heights disconnected from anything). So one could consider the workshop to be a success if it gave participants a clearer sense among:

the “lay of the land” in terms of how some ingredients fit together,
which parts of the prior work are truly relevant, and in what degree of generality, and
how the new notions introduced allow one to do things that cannot be readily expressed in more concrete terms.
The workshop helped with (i) and (ii), and to a partial extent with (iii).

It was reasonable that participants with advanced expertise in arithmetic geometry should get something out of the meeting even without reading any IUT-related material in advance, as none of us were expecting to emerge as experts (just seeking basic enlightenment). Many speakers in the first 3 days, which focused on material prior to the IUT papers but which feed into the IUT papers, were not IUT experts. Hence, they could not be expected to identify how their topic would precisely fit into IUT. It took a certain degree of courage to be a speaker in such a situation.

The workshop began with a lecture by Shou-Wu Zhang on a result of Bogomolov with a group-theoretic proof (by Zhang, if I understood correctly) that is not logically relevant (Mochizuki was not aware of the proof until sometime after he wrote his IUT papers) but provided insight into various issues that came up later on. Then there was a review of Mochizuki’s papers on refined Belyi maps and on elliptic curves in general position that reduced the task of proving ABC for all number fields and Vojta’s conjecture for all hyperbolic curves over number fields to the Szpiro inequality for all elliptic curves with controlled local properties (e.g., semistable reduction over a number field that contains sqrt{-1}, j-invariant with controlled archimedean and 2-adic valuations, etc.). This includes a proof by contradiction that was identified as the source of non-effectivity in the constants to be produced by Mochizuki’s method (making his ABC result, if correct, well-suited to finiteness theorems but with no control on effectivity).

次の講演は遠アーベル幾何に関するものだった（p進体・代数体上の双曲線や，そして様々な数論的基本群からの幾何的対象の「復元」定理に関するもの）．多くの講演のスライドはワークショップのページから見ることができる．

3日目は2つの Frobenioid に関する講演から始まった．この対象は望月によって2005年頃に最終的に必要なものを超えた非常に一般的なレベルで定式化された．Frobenioid は fibered category の一種で，（ある特殊例において）retains information related to pi_1 and line bundles on all finite etale covers of a reasonable scheme, but its definition involves much less information than that of the scheme．Frobenioid はまた，include a feature that can be regarded as a substitute for missing Frobenius maps in characteristic 0．水曜日の Frobenioid に関する講演は最終的にどの特殊な Frobenioid が必要であるのかを具体例付きで示した．

3日目最後と4日目最初の講演は，「エタール・テータ関数」に関する Kedlaya の重要な講演だった（従って，これはまだ IUT 理論の前段階の論文である）．Kedlaya の講演では非常に重要なことがわかった：p進テータ関数に関するあるコホモロジー的な対象の構築についてである（付録参照）．望月の深い遠アーベル的定理に基づいて，Kedlaya はこのコホモロジー的な対象を用いれば，Szpiro 予想に関する「全ての情報」が適切な Frobenioid によって保持されるという，非常に非自明な結果を概説した．従って，残りの仕事は，この Frobenioid 理論的な帰結を用いて何か重要な結論を得ることに変わったわけである．

しかし Kedlaya の講演以降の，IUT 論文本体に関する講演は，既に IUT を理解した参加者以外には理解できなかった：新しい記号，言い回しや用語が次々と導入され，IUT を既にある程度理解した人以外は完全に迷子になってしまった．この結末は，IUT 論文の正しさという数学的な問題には関係ない．しかし，数多くの数学者がこの論文を理解しようとしてできなかった原因を端的に示している．上記のワークショップの Web サイトに掲載された講演資料を見れば，たいていの数学者は参加者だったらどのように感じるか理解できるだろう．


# 5. 聴衆のフラストレーション

最後の2日間は，聴衆にとってかなりフラストレーションがたまるものだった．具体例を示そう．

私たちは「これらの2つの対象が準同型であるとしよう」だとか，あるいは「圏 D の 2 つのコピーを考え，異なるラベルをつけよう」といったような意味不明に思えることを繰り返し聞かされ続けた．何度も非常な苛立ちとともに質問がなされたが，最終的な目標のためにこのような方針が重要となることが納得できる具体例は提示されなかった．

しばしば私たちは p 進体の絶対 Galois 群が体論では生じないような自己同型を持つことに注意を喚起させられたが，なぜそのようなエキゾティックな自己同型の存在が Szpiro 予想の証明において重要なのかについて明快に説明されなかった．おそらく理由は簡単なものだと思うが，幾度も質問が出たにもかかわらず明確な回答はなかった（大抵「後でわかる」と言われたが，結局わからなかった）．

このような講演が続いた後，（驚いたことに）「例を提示しました」等々と言われた（本当に？興味深い例を？どこで？）．まるで「準同型な2つのベクトル空間を考えよう」と言い，いくら質問されてもそのような状況の面白い具体例を（数多く存在するにもかかわらず）一切提示せず，最後に「例は述べた」と言われる線形代数の講義のようだった．

聴衆からの数々の質問は，最後の2日間立ち籠めていた霧を取り除くには至らなかった．参加者は具体例（たとえ数学的構造の例でもよいので，わかり易いもの）を求め続けたが，聴衆にとって満足のいくような例は提示されなかった．

例えば私たちは（たいへんな早足で）非常に込み入った「Hedge 劇場」という数学的対象の定義を見せられたが，なぜこのような込み入った定義が必要なのかという理由を明確に説明されなかった（おそらくどこかで説明されたのだとは思うのだが，休憩時間中に質問した人々は理解できていなかった）．

Frobeinoid に関する一般論は究極的には不要であることがわかった今，Hodge 劇場の構築に必要な膨大な量のデータについても同じことが成立するのではないかというのは自然な疑問と言えるだろう；どの点が重要で，ある部分を取り除いたらどこで問題が生ずるのか明確に示されたならば，色々な部分で大きく事態は好転したはずだ．

聴衆が何度となく基礎的な質問をしたために講演が後ろ倒しになり，講演のなかにはスケジュール通りに進めるために早足になったものもあった．この結果としてより混乱が生ずるという悪循環が生じたとはいうものの，基礎的な質問が数多く出たのは最初の「情報量が多すぎる」問題によるものだ．講演は目の前の聴衆のためのものなのである．


# 6. おわりに

週の終わりにかけて生じた上記のような色々な難点や聴衆一般のフラストレーションにも係らず，このワークショップはいくつかの理由から実り多いのだった．このワークショップを通じて，鍵となる概念や定義の理解が進んだ．加えて，IUTの前段となる研究の発想に関する様々な興味深い議論の機会をもたらしたのみならず，IUTにアプローチするより効率的な道筋を明確にした（例えば，先行する論文の不要な部分をどのように避けていくか）．このワークショップはまた証明が effective ではないことの再確認ともなったし，肝となるコホモロジー的対象，また Frobenioid に関する重要な定義も明確にした．

もう一つの忘れられない特徴は，星裕一郎の専門性が存分に発揮されているのを見たことである．彼は講演者の誤りを直ちに修正することができたし，聴衆の質問に真摯に答えようと努力していた（講演者が聴衆が満足するレベルで答えられない質問は常に彼にまわされた）．

If the final 2 days had scaled back the aim to reach the end of IUT and focused entirely on addressing how the Frobenioid incarnation of the cohomological construction from Kedlaya’s lectures makes it possible (or at least plausible) to deduce something non-trivial in the direction of Szpiro’s Conjecture (but not necessarily the entire conjecture) then it would have been more instructive for the audience. Although “non-trivial” is admittedly a matter of taste, I do know from talking with most of the senior participants that most of us did not see where such a deduction took place; probably it was present somewhere in a later lecture, but we were so lost by everything else that had happened that we missed it.

I don’t understand what caused the communication barrier that made it so difficult to answer questions in the final 2 days in a more illuminating manner. Certainly many of us had not read much in the IUT papers before the meeting, but this does not explain the communication difficulties. Every time I would finally understand (as happened several times during the week) the intent of certain analogies or vague phrases that had previously mystified me (e.g., “dismantling scheme theory”), I still couldn’t see why those analogies and vague phrases were considered to be illuminating as written without being supplemented by more elaboration on the relevance to the context of the mathematical work.

At multiple times during the workshop we were shown lists of how many hours were invested by those who have already learned the theory and for how long person A has lectured on it to persons B and C. Such information shows admirable devotion and effort by those involved, but it is irrelevant to the evaluation and learning of mathematics. All of the arithmetic geometry experts in the audience have devoted countless hours to the study of difficult mathematical subjects, and I do not believe that any of us were ever guided or inspired by knowledge of hour-counts such as that. Nobody is convinced of the correctness of a proof by knowing how many hours have been devoted to explaining it to others; they are convinced by the force of ideas, not by the passage of time.

The primary burden now is on those who understand IUT to do a better job of explaining the main substantial points to the wider community of arithmetic geometers. Those who understand the work need to be more successful at communicating to arithmetic geometers what makes it tick and what are some of its crucial insights visibly relevant towards Szpiro’s Conjecture.

It is the efficient communication of great ideas in written and oral form that inspires people to invest the time to learn a difficult mathematical theory. To give a recent example, after running a year-long seminar on perfectoid spaces I came to appreciate that the complete details underlying the foundational work in that area are staggeringly  large, yet the production of efficient survey articles and lectures getting right to the point in a moderate amount of  space and time occurred very soon after that work was announced. Everything I understood during the week in Oxford supports the widespread belief that there is no reason the same cannot be done for IUT, exactly as for other prior great breakthroughs in mathematics. There have now been 3 workshops on this material. Three years have passed. Waiting another half-year for yet another workshop is not the answer to the current predicament.

For every subject I have ever understood in mathematics, there are instructive basic examples and concise arguments to illustrate what is the point to generally educated mathematicians. There is no reason that IUT should be any different, especially for the audience that was present at Oxford. Let me illustrate this with a short story. During one of the tea breaks I was chatting with a postdoc who works in analysis, and I mentioned sheaf theory as an example of a notion which may initially look like pointless abstract nonsense but actually allows for very efficient consideration of useful ideas which are rather cumbersome (or impossible) to contemplate in more concrete terms. Since that postdoc knew nothing about what can be done with sheaf theory, I told him about the use of sheaf cohomology to systematize and analyze the deRham theorem and topological obstructions to construction problems in complex analysis; within 20 minutes he understood the point and wanted to learn more. Nobody expects to grasp the main points of IUT within 20 minutes, but if someone says they understand a theory and does not provide instructive visibly relevant examples and concise arguments that clearly illustrate what is the point then they are not trying hard enough. Many are willing to work hard to understand what must be very deep and powerful ideas, but they need a clearer sense of the landscape before beginning their journey.
