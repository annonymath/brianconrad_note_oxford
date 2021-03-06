_This document is an unofficial Japanese translation of [Notes on the Oxford IUT workshop by Brian Conrad](http://mathbabe.org/2015/12/15/notes-on-the-oxford-iut-workshop-by-brian-conrad/). The translation is done in the aim of making the contents of the article, and hence the outcomes of the Oxford IUT workshop, accessible for a wider audience in Japan. The author of this document does not have the right to translate the article and is ready to remove the file upon request of the copyright holder._

[この試訳に関するおことわりなど](https://github.com/annonymath/brianconrad_note_oxford/blob/master/README.md)

--

# Brian Conrad によるオックスフォードでの IUT ワークショップのノート（試訳）

_Brian Conrad はスタンフォード大学数学科の教授であり、望月のABC予想に関する研究をめぐってオックスフォードで開催されたワークショップに参加した。彼は、ABC 予想の幾何学的定式化（これが望月が調べた問題である）を与える数論の一分野、数論幾何学の専門家である。_

_様々な人から幾度となくワークショップの感想を尋ねられたことから、Brian は以下のまとめを書いた。彼は、非専門家でも現在の状況から何か学ぶところがあるのではないかと期待している。Nature や Quanta に今後登場する記事は、より一般向けの内容となる見込みだ［実際の記事 → [Nature](http://www.nature.com/news/biggest-mystery-in-mathematics-in-limbo-after-cryptic-meeting-1.19035?WT.mc_id=FBK_NatureNews), [Quanta](https://www.quantamagazine.org/20151221-hope-rekindled-for-abc-proof/)］。この文書の構成は次の通りである：_

  1. 背景
  2. 基本的な考え方の理解を遅らせたのは何か？
  3. 宇宙際 Teichmüler 理論 (IUTT = IUT) とは何か？
  4. ワークショップで何があったか？
  5. 聴衆のフラストレーション
  6. 終わりに
  7. 技術的付録

## 1.  背景

ABC 予想は、およそ 30 年前に定式化されたばかりの予想ではあるが、数論における最も重要な予想のひとつである。複数の定式化が存在するが、そのうちには数論における際立った有限性定理やその他の結果に繋がるものや、或いはこの予想を証明するにあたって頑健な系統的アプローチを与えうる定式化がある。ABC 予想は、任意の正整数ペア（A と B）とその和（C）について、それらの数たちの素因数と実際の大きさとを結び付ける不等式に関する予想である。ABC 予想には、より大きな数の体系（「代数体」と呼ばれ、数論において常に現れる）上への自然な拡張が存在する。

自然数を対象とした場合のこの予想の正確な定式化と、この予想からの理論的帰結に関しては [Wikipedia](https://en.wikipedia.org/wiki/Abc_conjecture) で議論・説明されている。重要な応用例も自然数の場合において述べられている。ABC 予想に現れるような自然数の乗法的性質と加法的性質の相互作用は、やや繊細な問題である（例えば、_p_ を素数としたとき、_p_ + 12 の素因数分解について非自明なことは何も言えない）。この予想で現れる不等式には、uniform control の度合いを表現する補助的定数が含まれており、これによって多くの条件下で特筆すべき帰結をもたらす。そのほかの理論的帰結については、[このページ](http://www.math.unicaen.fr/~nitaj/abc.html#Consequences)にリストアップされている。

ABC 予想が重要な理由は、定式化された当初には予想もされていなかった多くの豊富な理論的帰結を持つからである（この予想とそのもたらす結果の多くについては、代数体上での定式化に一般化した議論が不可欠である）。

1980 年代半ばに定式化された時点から、ABC 予想が他の重要な未解決問題と深いつながりがあり、また時に等価であることは知られていた。例えば Mordell 予想に対する effective な証明を挙げられる（「大きな種数」をもつ代数曲線の有理点の数を明示的にバウンドすること。単に有理点の数の有限性を示すより遥かに難しい；なお Mordell 予想は、このような点の集合が有限個しかないことを主張するものであり、Faltings によって 1980 年代に証明された。Faltings はこの成果によって Fields 賞を授与された）。Modell 予想に対する effective な証明を導くためには、ABC 不等式に現われる定数を明示的に求める必要がある。

他の等価な定式化には「楕円曲線」を用いるものがある。楕円曲線とは、2 変数 3 次方程式によって定義される曲線であり、数論における数多くの問題（特に、Fermat の最終定理を含む）に登場する。Lucien Szpiro は、楕円曲線の不変量に関してある不等式が成立することを予想した（Szpiro 予想）。ABC 予想が David Masser と Joseph Oesterle によって定式化されてから暫くしてのち、任意の代数体上での定式化に一般化すれば、ABC 予想と Szpiro 予想とは等価であることが知られるところとなった（この事実は「Frey 曲線」と呼ばれる、Fermat の最終定理と楕円曲線とを関係づける際にも用いられるある特別なクラスの楕円曲線を用いて証明される）。

望月新一は Faltings のもとで 1992 年に Ph.D. を取得して以来、京都の 数理解析研究所 (RIMS) で研究を続けている優れた数学者である。彼がこの問題を長期的な達成目標として、少しずつ彼の専門分野（数論幾何、特に遠アーベル幾何）において様々な深い技術的進展を積み上げていることは長きにわたって知られていた。望月のアプローチにおいては、Fermat の最終定理に対する証明がそうだったのと同様、この予想に関して何らかの結果をもたらすためには、当初の定式化にあるような具体的な数同士の関係を直接取り扱うことはしない。かわりに、具体的な数値的データを取り扱うのでは到底利用不可能なより強力な道具や操作を利用可能にするため、ABC  予想は数論幾何学におけるより精巧な理論的枠組みに基づいて再定式化される。望月の目標は Szpiro 予想の証明だった。

2012 年 8 月、望月は「宇宙際 Teichmüller 理論」と彼が呼ぶ理論によってこの予想を解決したと宣言し、Szpiro  予想の証明で終わる長いプレプリント群を公開した。望月は際立って優れた（そして、非常に注意深い）数学者であり、また彼の ABC 予想に対するアプローチ（楕円曲線に関する Szpiro 予想を経由するアプローチ）は、遠アーベル幾何学において彼自身がこれまでに編み上げてきた深い幾何学的・群論的理論の壮大な絵巻物に基づくものである。長い期間にわたって、この問題を解決するための道具の構築と応用に相当の労力を費してきたことに関して、彼は尊敬されて然るべきである。

望月の今現在の手法では、ABC 不等式の定数を明示的に得ることは**できず**、Mordell 予想の effective な証明は構成できない。しかしいずれにせよ、この証明が正しいとすれば、様々な未解決の難問を解決するとともに Mordell 予想の新たな証明となる（この点はずっと昔に Noam Elkies が証明している）。驚異的な成果だと言える。

専門家たちは直ちに、望月の証明が正しいか検証するのが非常に難しいと理解した。証明が書かれている論文は、非常に多くの見慣れない用語や記法、具体例なしの定義の羅列が続く形式で書かれており、数論幾何学に関する十分な知識を持つ読者でさえもこの論文を読み進めようとするにあたって自分が確かに進んでいるという感覚を得られなかった。論文にはアナロジーやモチベーションを述べる数多くの注釈が存在するが、初めて読む多くの読者にとってはこれらの注釈の重要性や、アナロジーの意味を理解するのは難しかった。普通の論文に比べて「モチベーション」に関する議論が非常に多いことからすれば逆説的であるが、多くの読者はすぐに意欲を失うか或いは混乱してしまい、読むのを止めてしまった。論文本体を読む困難さに加え、望月はメールでの質問には意欲的に答えるとともに RIMS への直接の訪問者との議論には応ずるものの、出張や講演をしなかった。

今日に至るまで、遠アーベル幾何に基づいて ABC 予想を証明しようとする彼の発想を普及させ検証する上では多くの課題が残っている。長いあいだ状況を停滞させる要因となっていたのは、数論幾何コミュニティに属する多くの人の意欲が削がれていたことだ。こうした状況は、[Nature の記事](http://www.nature.com/news/the-biggest-mystery-in-mathematics-shinichi-mochizuki-and-the-impenetrable-proof-1.18509)で説明されている。

最初の発表から3年が経過したとは言うものの、この時間のあいだ数論幾何学者がみなこの論文の検証を続けていたというわけではない。どちらかと言えば、多くの人が初期に挑戦し、すぐに意欲を失ってしまった（新奇な記号、用語、考え方が余りに多過ぎたのも原因のひとつだ）。サーベイ論文も数本書かれたが、私が話したほぼ全ての数学者が、これらのサーベイから啓蒙を得るのはもとの論文と同様に難しいと述べた（なかには理解が進んだという人もいたが、多くはそうではなかった）。

クレイ数学研究所 (CMI) とオックスフォード大学数学研究所は、重要な一歩を踏み出すのに貢献した。ABC 予想に関連する数論幾何学の諸分野の専門家（宇宙際 Teichmüller 理論を検証してはいない）を集め、望月の研究に関するワークショップを開催したのである。専門家集団として、数学者個々人ではあまりに意欲を削がれてしまって成し遂げられなかった、理論の大枠についての理解を進展させようと目指したのである。このワークショップを開催するために尋常でない労力を費した主催者たち［Ivan Fesenko, Minhyong Kim, Kobi Kremnitzer］は、（CMIの スタッフたちもあわせ）賞賛されるべきである。ワークショップを開催するために十分な講演者を集めるのは困難を極めた。多くのベテランは講演したがらなかったし、また講演者の多くにとっては望月の研究対象（例えば Frobenioid やエタール・テータ関数）はまったく新規なものだった。講演者の多くが、自分の話す内容が最終的に全体の流れのどこに位置するかしばしばわかっていなかったのも理解できることだ。狙いは、ひとりひとりの努力が組合わさることで、全体としての理解が進むのではないかということだった。

私はこのワークショップに参加した。参加者のうちには Alexander Beilinson、Gerd Faltings、Kiran Kedlaya、Minhyong Kim、Laurent Lafforgue、Florian Pop、Jakob Stix、Andrew Wiles、そして Shou-Wu Zhang といった、著名な数論幾何・遠アーベル幾何の研究者もいた。全参加者のリストは[ここ] (https://www.maths.nottingham.ac.uk/personal/ibf/files/symcor.iut.html)に公開されている。

証明の正しさを検証するのはワークショップの目的ではなかった。私の（そして他の多くの参加者の）理解では、このワークショップの目的は、数論幾何の様々な分野から集まった参加者が、望月の研究全体の鍵となるアイデアについて理解を深めること、（そして特に）望月の論文を読もうとするにあたって多くの数学者が感じた、意欲を削がれる感覚を緩和することだった。

望月の研究は、深い着想に基づいて新しいツールを構築・分析し、ABC  予想に対する新たなアプローチを与えるものだ（ツールたちそれ自体は、完全に通常の代数幾何学に即している）。ただし、数学において難解な証明の正しさを検証する上では、様々な理解の段階がある。その最初の段階は、優れて新しい着想がどこにあるか、またそれがおおよそどのようにして結果をもたらすのかという点についての明確な理解である。現状では、望月の研究に関してはそのような理解が（少なくとも数論幾何学の研究者の多くにとって納得のいくレベルでは）存在しない。これが、彼の主論文で何がなされたのか現在でも広く理解されていない主要因となっていた。このような「主たる着想の理解」という方向性について、ワークショップは確固たる進歩を成し遂げたといえ、その意味で有益なものだった。

ワークショップを通じて、多くの人が望んでいた「アハ！」体験は存在しなかった。しかし私は、週の後半にかけて蓄積した強いフラストレーションにもかかわらず、このオックスフォードでのワークショップに参加してよかったと思っている。多くの参加者は、理論の部分部分や、主な課題がどこに存在するのかに関して理解を深められたが、宇宙際 Teichmüler 理論に関するエキスパートにはなれなかった（これはワークショップの目標ではなかったとは思う）。ワークショップの発表を通じて、様々な理論や中間的な結果が相互に深く関係し合う様子や、望月の様々な過去の結果が色々な部分に入り込んでくる様子が見られた。彼が注意深くかつパワフルな数学者であるというこれまでの記録も考えに入れれば、彼の研究は真剣に検証されるべきものであると言える。

「聴衆」の意見や期待に関する下記の記述は、（一般に宇宙際 Teichmüler 理論の専門家ではない数論幾何の専門家である）参加者たちと私が交わした会話に基いている。私の知る限りでは、ワークショップに関する期待や、この一週間で何が起こったかの感想について、参加者の考えは一致しているようだ。この文書に書かれていることの不正確性は、究極的には私の責任である。修正があれば歓迎です（効率のため、コメント機能を使ってください）。


## 2. 基本的な考え方の理解を遅らせたのは何か？

彼の論文の前提となっている研究が長い年月にわたってなされていることは、主たる着想が広く理解される上で妨げとなった。しかもこの長い年月のあいだ、研究のどの部分が最終的に、つまり主定理の証明のみを理解するために、必要となるのかわかっていなかった。これまで、主たる定理を導くための論理の流れが明快にわかるような用語・記号の定義を用いて一貫した議論を与えるといった「掃除」はなされていない。（最終的には）こうした掃除が必要だ。

望月は、代数体上のあらゆる楕円曲線に関する Szpiro 予想の証明（定数が代数体の次数と、ε のみに依存するもの）を目的としている。この予想からより具体的な結果（例えば ABC 予想、そして従って様々な有限性定理：Mordell 予想、アフィン曲線の整数点に関する Siegel の定理、そして、適当な代数体上でほとんど全ての点で良い還元を持つ楕円曲線の有限性）を帰結させる方法は何十年も昔から知られており、彼の議論においては一切登場しない。従って特に、このような具体的結果に依存する議論によって望月の手法が正しいかどうか「試す」ことはできない。彼の全ての議論は Szpiro 予想の文脈でなされているからである（この文脈では、具体的な結果は一切関係しない）。

しかも、彼の手法は対象とする楕円曲線に関してある大域的・局所的性質を要求する（例えば、split 30-torsion をもち、かつ全ての bad places で  split multiplicative reduction を持つなど）が、これらの性質は Frey 曲線は一般に満足せず、適切な次数をもつ基礎体の拡大において満足される。彼はこうした特殊例を用いつつも、こうした特殊例から一般の場合（なんと任意の代数体！）に拡張可能な短いが賢い主張を抽出する。が、その代償として、定数を明示的に求められなくなる。従って、彼の手法を有理数の集合のような小さな基礎体で直接適用することはできない；有理整数に関するもともとの不等式は、比較的大きな（しかし適切な）次数を持つ代数体における結果から従うのである。

時には IUT より以前に発表された望月の他の論文、一般の数学者にとっては不慣れな内容（Frobenioid や anabeliod）に関する論文への参照がなされ、数多くの新しい概念を理解する必要に迫られる。この結果として無限退行するかのような印象が生み出され、これもまた意欲を削ぐ効果をもたらした。しばしば望月の議論は一般論から具体論へ進むという形をとるからである（論理としてはよいだろうが、新しい概念を学ぶ際には必ずしもよい順序とは言えない）。例えば、もし望月の理論における Frobenioid（この単語は「Frobenius」と「monoid」の合成語である）という重要な概念を理解しようとしたとき、この概念を構築しようとするモチベーションが、彼の楕円曲線に関する Hodge-Arakelov 理論の研究から来ていることがわかる。しかし、この結果として 2 つの（数学的なというよりは）心理的な障害にぶつかる：
  1. Hodge-Arakelov 理論は最終的には使われない（数論的な 小平-Spencer 理論を構築することが、関数体の場合に触発された望月の当初の狙いであったが、このアプローチは失敗した）。最終的には使われないとしたら、ただモチベーションを理解するためだけに、どれだけの時間を非自明な理論の学習に費すべきなのだろうか？（もし費すとしたら、だが）
  2. Frobenioid の理論に関するほとんどの部分（望月の、IUT より以前に発表された 2 つの論文の内容）も、最終的には使われない（特殊例のみで十分である）。しかし、初めて学ぼうとした読者は気付かないかもしれず、全ての理論を理解しなければならないと（誤って）思い込むかもしれない。望月の Web ページに、究極的にはこの理論のほとんどが使われないことを述べている短い注釈があるが、独学中の数学者は気付かないかもしれない。たとえこの注釈を発見し、これらの論文のうち最終的に使われる重要な特殊例を取り扱った部分のみを読もうとしても、膨大な記号・用語や、前の方で述べられている結果が使用されているのを目のあたりにすることになる。こうして、「特殊例を理解するためだけでも、結局のところ最も一般的な議論を理解するために最初から読まなければならないのではないか」という恐怖を（間違ってはいるものの）感じ、結局は意欲を失ってしまうかもしれない。

これは Grothendieck のエタール・コホモロジーを学ぶときのことを思い起こさせる。近年では、この理論を一から直接的かつ（多かれ少なかれ）効率的なやりかたで構築し、重要な定理を証明していくようなよい本がいくつかある。数分冊に渡る SGA4 における Grothendieck の定式化では、非常に抽象的なトポスの一般理論を構築するために最初の何百ページもが割かれている。これは後の様々な一般化のための基礎となることを目指して書かれていた（そして後に実際に一般化された）。このような非常な一般性はしかし、エタール・コホモロジーのみを理解しようとするためには（任意の圏を理解するためにさえも）完全に不必要である。


## 3. 宇宙際 Teichmüler 理論 (IUTT = IUT) とは何か？

IUT のおおよその定義を、私の理解に従って順々に述べていく。望月が Szpiro 予想（従って ABC 予想）を証明する手法は、動機としては、この予想に登場する楕円曲線の鍵となる数論的不変量を「対称性」のみによって（従って元の楕円曲線に直接言及することなしに）記述しようとするものである。これは、付随するある幾何的対象の（数論的）基本群によって与えられる群論的データを用いることによって達成される。このようなものは Grothendieck の遠アーベル幾何における予想に現れ、Grothendieck 予想については望月自身によって目覚ましい結果が得られている（Grothendieck が予想しようとすら思わなかった結果までもが示された）。この手法は付録に掲載した；この手法は、完全に通常の数論幾何・非アルキメデス的幾何における議論を用いる（_p_ 進テータ関数、直線束、Kummer 射像、そして基本群の Heisenberg 型 subquotient を用いる）。

望月の戦略は、Szpiro 予想を完全に群論的で「離散的」なものに再定式化する（つまり、特定の代数的・幾何学的対象から離れ、群論的・圏論的な対象が組み合わさった構造に関心を移す）ことだ。これによって、直接は幾何学的な解釈が存在しない操作を加えることが可能となる。またこの結果として、結論はもとの幾何学的状況設定では解釈できなくなる。

大雑把なアナロジーとしては、Wiles の Fermat の最終定理 (FLT) の証明においては、Fermat の方程式を直接取り扱うことはしないし、Frey が仮想的な反例を埋め込んだ楕円曲線すら直接取り扱わない。その代わりに、Wiles は Galois 表現を変形する、より広い枠組みに再定式化し、楕円曲線そのものでは表現できない（可換環論と Galois コホモロジーに由来する）別のテクニックや操作を可能とした。より望月自身の研究に即したアナロジーとしては、_p_ 進体の絶対 Galois 群は（代数体のそれとは異なり）体論的な自己同型にはない（トポロジカル）自己同型を持ち、従ってある代数体をその絶対 Galois 群で置き換えたときには新しいことが起こり（「エキゾティックな」自己同型が現れる）、もとの代数体ではこれは表現できない。

より具体的には、望月が導入した枠組み、Frobenioid 理論は、群論的データと層論的データの組み合せによって、標数ゼロの数論幾何構造に対する「Frobenius 写像」という古くからの夢を部分的に実現するものである。これを如何に実現するかという着想は、望月の _p_ 進 Teichmüller 理論に関する過去の研究から来ているようである（従って「IUT」の「Teichmüller」になっている）。様々な幾何的対象について望月は「Frobenioid」を対応させ、然る後に幾何的対象を捨て去って完全に Frobenioid たちのみを用いた議論に移行する。FLT とのアナロジーで言うならば、Wiles は Galois 表現を得るや否や楕円曲線を投げ捨て、もとの楕円曲線においては何ら意味を持たない、Galois 表現に関する議論を進めている。

Frobenioid と、Frobenius 写像やその他の「非幾何学的な出自を持つ」操作との類似は、楕円曲線の数論的不変量を保持する Frobenioid から非自明な情報を取り出す上で本質的であるようだが、私には理解できなかったし、オックスフォードでのワークショップでも明快に説明されなかった。恐らく最後の 2 日間の講演のどこかに埋もれていたのだろう；この点を理解するのは、IUT においてどこに幾何学と数論との深い繋がりが現れるのかを理解する本質的な一歩になるように思われる。

まとめると、IUT は、第一近似としては、Frobenioid たちの操作や Frobenioid を用いた対象を調べる理論であり、幾何学的考察以上の表現能力を有している。そして、この理論を楕円曲線の不変量を保持した Frobenioid に適用することで、興味深い結論が得られる。「IUT」の「IU」の部分は、Szpiro 予想の証明自体には不要とみられる、より技術的なものである。

結論としては、難しい数学的問題に取り組む研究においてよくあるように、もともとの具体的な問題設定では表現しづらい構造を把握するため、まず視野を拡張するのである。これは一種賭けのようなもので、一般化した問題／状況設定は証明したい内容が正しいとしても破綻し得る；例えば、Wiles の FLT の証明において、変形環と Hecke 環の準同型を示そうという目標は、これは要求される結果からは強すぎるものだが、しかし当初の手法では必要とされた一般化だった。（のちの Wiles の手法の改善によって、この問題を避け、準同型ほど強い結論を得ずとも最終的な数論的帰結を導くように強化された）

望月の Szpiro 予想に対するアプローチと Wiles の FLT の証明とのひとつの大きな違いは、後者は特殊例に限っても注目すべき部分的な結論が存在したことだ。 例えば判別式が素数の楕円曲線がある。一方 IUT は、簡略化された方法に基いて導かれる ABC 不等式よりは弱いが興味深い不等式といった特殊な例を持たない（また、どうやら具体的な ABC 予想の結果を用いて、IUT の「性能を確認」することもできないようだ）。Skype セッションで望月はまさにこの質問を受けたが、そのような可能性は思い付かないと答え、彼の手法は「all or nothing」のように思われる、と付け加えた：IUT は求めたい不等式を自然な形で導くが、この手法を弱めた場合には弱い特殊例を導くのではなく、単に何も生み出さないということだ。

以下では、「宇宙際」という言葉の意味について考える。彼の IUT 理論の研究において「宇宙」に関する議論があることから、彼の証明が（もし正しければ）本質的な形で巨大基数や Grothendieck 宇宙といった集合論の微妙な話題に依存しているのではないか、あるいは新しい数学の基礎付けを要求しているのではないかという関心があった。以下では、この考えが誤っていると私が信ずる理由を説明する（ただし、望月の宇宙に関する考察は、より理論を一般化する上では意味がある）。

望月が宇宙たちに関する議論に取り組んだ理由は、彼の理論の重要部分から生ずる厄介な表現上の問題を回避するために、完全に一般的な条件における定式化を考えたことによって生じている（大雑把には次の通り：幾何学的・あるいは体論的データに関する profinite group からの定量的見積りを可能にする形での「復元定理」とは、正確には何を意味するのか？）。このような議論をする十分な理由はあるものの、こうした一般的な状況設定は、彼の証明を一歩一歩追ったり、Szpiro 予想の証明に十分なだけ理解する上では不要のように思われる。

Grothendieck は SGA4 において、まず一般のトポスに関する厳密な理論を構築し、その際に宇宙を導入した。このトポスの一般論は、エタール・コホモロジーを導入するための前奏曲だった。しかし、エタール・コホモロジーの主要な定理群を理解している数学者ならば、これらの定理群自体のために「宇宙」は不要であることを知っている。これは厳密でない議論を許すということではなく、証明の主要なアイデアを理解しているということだ。Grothendieck はスキームのエタール・トポスという特殊ケースにおいてのみ証明を与えるのではなく、トポスの一般論に基づいて彼の理論を構築した。しかし、必ずそのように議論を進めなければならないわけではない（エタール・コホモロジーに関する学術書を見ればわかるよう、宇宙は一切用いられないが証明は完全に厳密である）。

換言すれば、厳密な「万物理論」を構築するために必要なものは、「何かの理論」には必ずしも必要ではない。望月は「宇宙のとりかえ」について第 4（そして最終）論文で相当の議論を加えている（これは「宇宙際」という言葉が「IUT」に含まれている主要な理由であると思われる）。しかし、宇宙に関するこのような議論は、何か他の用途で用いるための非常に一般的な理論を構築するうえで現れたものであって、Szpiro 予想を示すのに十分か否かという意味で言えば、不必要な議論である。「車輪の再発明」をすることなしに、IUT の将来的な発展を見越した強化を目指す目的であれば、「宇宙際」の議論は必要なのかもしれない。ワークショップの参加者で、モデル理論がこうした問題については十分成熟した枠組みになるだろう、と発言していた人もいた。しかし、数論的応用（特に ABC 予想）を考える上では、この部分は関係がないとみられる。

## 4. ワークショップで何があったか？

ワークショップの講演スケジュールは、理論全体の概観を与えることを目指していた。私が言葉を交わした参加者は皆、楕円曲線の高さの理論（Szpiro 予想の本質的特徴）と、望月の遠アーベル幾何の研究との重大な接触がどこで生ずるのかを理解しようとしていた。特に、このような接触が（単に、どんな対象とも一切関係ない、高さに関する新しい不等式を得るのではなく） Szpiro 予想の方向に向かうような洞察を与える部分で生ずるのかどうかに注目していた。従って、次の点について参加者が明快な理解に達したとしたら、このワークショップは成功と言えた：

  1. 色々な要素がどう組み合わさるかという「地勢図」、
  2. 前提となる IUT 以前の研究について、どの部分が本当に重要で、どの程度の一般性が要求されるのか、そして
  3. 新たに導入されたものによって、より具体的な方法では実行不可能な、どのようなことが可能となるのか。

ワークショップは (1) と (2) について成果をあげ、 (3) については部分的に成果をあげた。

私たちの誰もが IUT の専門家としてワークショップに登場することを期待されていたわけではない（ただ基本的な啓蒙を得ようとしていたのである）。事前に IUT 関係の論文を読まなくとも、数論幾何学の秀でた専門家である参加者たちならば、何かを得ることができるはずだった。最初の 3 日間の講演者たちは IUT に繋がる IUT 理論の前段階の論文を読んだが、彼らも IUT の専門家ではない。従って、彼らは自分たちの講演が IUT のどこにおさまるのか理解していることは期待されていなかった。こうした状況下で発表するのは、発表者にとっては勇気がいる。

ワークショップは、Show-Wu Zhang の Bogomolov による群論的証明に関する講演から始まった（Zhang によるものだったと思う）。この講演は、論理的には IUT と関係しない（望月は IUT 論文を書いて後しばらく経つまでこの証明を知らなかった）が、後々の講演では様々な点において洞察をもたらした。その後、望月の 一般の楕円曲線に対する refined Belyi 写像に関する講演があり、ここでは任意の代数体上のABC予想と任意の双曲線に対する Vojta 予想を、局所的な性質について制限付きの（例えば semistable reduction over a number field that contains _√-1_, _j_-invariant with controlled archimedean and 2-adic valuations など）任意の楕円曲線に対する Szpiro 予想に帰着させられることが示された。ここで背理法による証明が用いられており、これが望月の手法によって導かれる定数が effective でない理由となっている（このことによって彼の ABC 予想の証明は、もし正しいとすれば、有限性定理には適用可能であるが effective さについては何も言えなくなっている）。

次の講演は遠アーベル幾何に関するものだった（_p_  進体・代数体上の双曲線や、そして様々な数論的基本群からの幾何的対象の「復元」定理に関するもの）。講演のスライドの多くは[ワークショップのページから見ることができる](https://www.maths.nottingham.ac.uk/personal/ibf/files/iut-sch1.html)。

3 日目は 2 つの Frobenioid に関する講演から始まった。この対象は、Szpiro 予想の証明において最終的に必要となるものを超えた非常に一般的なレベルで、2005年頃に望月によって定式化された。Frobenioid はファイバー付き圏の一種で、（ある特殊な Frobenioid は）適切なスキームの有限エタール被覆に関する全ての _π_ _1 と直線束に関する情報を保持できるが、 しかしスキームのそれよりもかなり要求される情報が少ない。Frobenioid はまた、標数ゼロにおいて存在しない Frobenius 写像の代替物と見做すこともできる。水曜日の Frobenioid に関する講演は、最終的にどの特殊な Frobenioid が必要であるのかを具体例付きで示した。

3 日目最後と 4 日目最初の講演は、「エタール・テータ関数」に関する Kedlaya の重要な講演だった（これはまだ IUT 理論の前段階の論文である）。Kedlaya の講演では非常に重要なことがわかった：_p_  進テータ関数に関するあるコホモロジー的な対象の構築についてである（付録参照）。Kedlaya は、望月の深い遠アーベル的定理に基づいて、このコホモロジー的な対象を用いれば、Szpiro 予想に関する「全ての情報」が適切な Frobenioid によって保持されるという、非常に非自明な結果を概説した。従って、Szpiro 予想を証明するための残りの作業は、この Frobenioid 理論的な帰結を用いて何らかの重要な結論を得ることに変わったわけである。

しかし Kedlaya の講演以降の、IUT 論文本体に関する講演は、既に IUT を理解した参加者以外には理解できなかった：新しい記号、言い回しや用語が次々と導入され、IUT を既にある程度理解した人以外は完全に迷子になってしまった。この結末は、IUT 論文の正しさという数学的な問題には関係ない。しかし、数多くの数学者がこの論文を理解しようとしてできなかった原因を端的に示している。上記のワークショップの Web サイトに掲載された講演資料を見れば、たいていの数学者は参加者だったらどのように感じるか理解できるだろう。


## 5. 聴衆のフラストレーション

最後の 2 日間は、聴衆にとってかなりフラストレーションが積み上がるものだった。例を示そう。

私たちは「これらの 2 つの対象が同型であるとしよう」だとか、あるいは「圏 _D_ の 2  つのコピーを考え、しかし異なるラベルをつけよう」といったような、意味不明に思える内容を繰り返し聞かされ続けた。非常な苛立ちとともに何度も質問が出たが、こうした方針が最終的な目標を達成するために重要となることが納得できるような具体例は提示されなかった。

しばしば私たちは _p_ 進体の絶対 Galois 群が体論では生じないような自己同型を持つことに注意を喚起させられたが、なぜそのようなエキゾティックな自己同型の存在が Szpiro 予想の証明において重要なのかについての明快な説明はなかった。おそらく理由は簡単なものであるのだと思うが、幾度も質問が出たにもかかわらず明確な回答はなかった（大抵「後でわかる」と言われたが、結局わからなかった）。

このような講演が続いた後、（驚いたことに）「例を提示した」等々と言われた（本当に？興味深い例を？どこで？）。まるで「同型な 2 つのベクトル空間を考えよう」と言い、いくら質問されてもそのような状況の面白い具体例を（数多く存在するにもかかわらず）一切提示せず、最後に「例は述べた」と言われる線形代数の講義のようだった。

聴衆からの数々の質問は、最後の 2 日間立ち籠めていた霧を取り除くには至らなかった。参加者は具体例（たとえ数学的構造の例でもよいので、わかり易いもの）を求め続けたが、聴衆にとって満足のいくような例は提示されなかった。

例えば私たちは（たいへんな早足で）非常に込み入った「Hodge 劇場」という数学的対象の定義を見せられたが、なぜこのような込み入った定義が必要なのかという理由は明確に説明されなかった（おそらくどこかで説明されたのだとは思うのだが、休憩時間中に質問した人々は理解できていなかった）。

Frobeinoid に関する一般論は究極的には不要であることがわかった今、Hodge 劇場の構築に必要な膨大な量のデータについても同じことが成立するのではないか、というのは自然な疑問と言えるだろう；どの点が重要で、ある部分を取り除いたらどこで問題が生ずるのか明確に示されたならば、色々な部分で事態は大きく好転したはずだ。

聴衆が何度となく基礎的な質問をしたために講演が後ろ倒しになり、講演のなかにはスケジュール通りに進めるために早足になったものもあった。この結果としてより混乱が生ずるという悪循環が生じた側面はある。しかし、基礎的な質問が数多く出たのは最初の「情報量が多すぎる」問題によるものだ。講演は目の前の聴衆のためのものなのである。


## 6. おわりに

週の終わりにかけて生じた上記のような色々な難点や、聴衆一般のフラストレーションはあったものの、このワークショップはいくつかの理由から実り多いのだった。このワークショップを通じて、鍵となる概念や定義の理解が進んだ。加えて、IUTの前段となる研究の着想に関する様々な興味深い議論の機会を提供したのみならず、IUT にアプローチするより効率的な道筋も明確になった（例えば、前提となる論文の Szpiro 予想の証明には不必要な部分をどのように避けていくか）。このワークショップはまた証明が effective ではないことの再確認ともなったし、肝となるコホモロジー的対象や Frobenioid に関する重要な定義も明確になった。

もう一つ忘れられないのは、星裕一郎の専門性が存分に発揮されているのを見たことである。彼は講演者の誤りを直ちに修正することができたし、聴衆の質問に真摯に答えようと努力していた（講演者が聴衆が満足するレベルで答えられない質問は、常に彼にまわされた）。

もし最後の 2 日間の講義が、IUT を全部通して読むという大きな目標をより小さな目標にスケールダウンし、Kadlaya の講演にあったようなコホモロジー的対象の Frobenioid 化から Szpiro 予想の証明につながる非自明な結論がどのようにして得られるのかを示すことに注力したのならば（例えそれが証明全体を完成するというわけでなくても）、聴衆にとってはもっと理解しやすいものとなっただろう。「非自明な」というのは恐らく判断が分かれる問題だとは思う。しかし、ベテランの参加者ほぼ全員と話してみたところでは、皆そのような結果が得られた部分を見つけることはできなかったようだ；きっと後半の講演のどこかには存在したはずなのだが、我々はもう完全においてけぼりになっており、何かがあったとしても見逃してしまった。

最後の 2 日間でなされた質問に対して、より明快で理解しやすい形で回答できず、コミュニケーション障害を生じさせた原因が何かはわからない。確かに多くの参加者はワークショップの前に十分 IUT 論文を読んだわけではないが、これは説明にはならない。かつて私を当惑させたアナロジーや曖昧な表現（例えば "dismantling scheme theory"）の意味を私が理解した時でも（このような瞬間はこの週の間に何度かあった）、私はなぜそうしたアナロジーや曖昧な表現が、数学的文脈に基づくより詳細な補足的議論を追加するよりも分かり易いと言えるのか理解できなかった。

ワークショップの間、既に理論を理解した人が何時間費したか、あるいは A という数学者が B や C に対して何時間セミナーをしたかについて、何度かリストを見せられた。こうした情報はそれらの人の尊敬すべき労力を示してはいるものの、数学的内容を検証したり学習したりする上では意味がない。参加していた数論幾何学者たちは、数え切れない時間を難解な数学的理論を学ぶために費してきたわけであるし、私は上に書いたような時間数のデータが何かのガイドになるとは思わない。証明の正しさを、それを説明するために何時間掛かったかで判断する人はいない；時間の経過ではなく、考え方の力によって判断するのだ。

IUT を理解した数学者たちの責務は、より広い数論幾何学者コミュニティに重要な点を説明するために全力を尽くすことだ。理解している数学者は、証明がどのように動いており、何が Szpiro 予想につながる最も重要な洞察なのか、他の数論幾何学者に対してよりうまく説明する必要がある。

難しい数学理論を学ぶために時間を費そうと人々を動機付けるのは、文書および口頭で効果的に重要な考え方を伝えるコミュニケーションだ。最近の例を挙げるなら、perfectoid 空間に関する 1  年あまりのセミナーをやってみて私が気付いたのは、この話題に関して基礎となる理論の詳細はおそろしく膨大であるのにもかかわらず、要領のよいサーベイ論文や、時間・量ともに程々なレクチャが理論の公表後かなり早いうちに現れたことだ。私がオックスフォードにいた間に経験したことは全て、広く共有されている次の考えを支持している：数学においてこれまでなされた偉大なブレークスルーに対してできたように、IUT について上記のようなことができないとは思えない。これまで 3 回ワークショップが開催された。3 年が経っている。もう半年次のワークショップまで待つというのは、このような窮状に対する答えではない。

私がこれまで理解したどんな数学的内容についても、十分訓練を受けた数学者に対して重要な点を分かり易く示せる教育的で基本的な例や簡潔な命題が存在する。IUT が特殊だと考える理由は、特にオックスフォードのワークショップに参加したような人々を前提聴衆とするならば、ない。これを簡単な例で示そう。ティーブレイクの際、解析学を専門とするポスドクと話していた。私は、最初はまるで意味を欠く abstract nonsense だと思われたが、その実より具体的な手法では面倒な（あるいは不可能な）取り扱いを非常に効率化するような理論の例として、層論を挙げた。このポスドクは層論で何ができるのかまったく知らなかったので、私は彼に層コホモロジーを用いて de Rham の定理と複素解析における topological obstruction を統一的に取り扱い、分析する方法を説明した；20 分のうちに彼は理解し、もっと勉強したいと言った。誰も IUT の重要部分を 20 分のみで理解できるなどとは思わない。しかし、もし IUT を理解したという数学者が、教育的かつわかりやすい例や、重要な点を明快に示す簡潔な主張を提示できないのであれば、努力が足りない。深く強力な考え方に違いないものを学ぶためならば、誰もが全力で理解しようとするだろう。しかし彼らが旅立つ前に、これから歩を進めようとする場所の地形を頭に入れておかなければならない。

## 7. 技術的付録

［訳者の数学的背景の不足によって割愛します］

-- 
## コメント

* **Thimothy Chow:** ブライアン、星について高く評価していますね。彼（あるいは他の関係者）は、望月の Szpiro 予想の証明の詳細までチェックし、正しいと主張しているのですか？それとも証明の正しさを「断言」するのは避けているのですか？
  * **Brian Conrad:** ティム、私の記憶では、彼は全ての論理をフォローし正しいと信じていると語っていました。ただ、私たちが求めているのは数学者コミュニティとしての理解であって、これは現状の説明の方法ではなかなか達成できません。例えば、変化させるパラメタの正確で一様な制御が要求される計算では、間違いが生じやすいと思います。よりたくさんの数学者たちが検証に参加できるようにすれば、事態は劇的に変わると思います（例えば、あるステップからあるステップに進むためにどのような性質が要求されるのかの明確なリストを準備して、問題の分割を試みるのはひとつの手でしょう）。
    * **Marshall Flax:** アナロジーで語ってみましょう：Harry Potter の第１巻は短くてしっかりした編集でした。しかし第５巻になるころには、草稿をそのまま印刷したみたいになっていました。いい文章を放り捨てるのは心理的に難しいけれど、腕利きの編集者ならば、作家に対して読者のためにそうするよう求めるでしょう。しかし第５巻のころには J. K. Rowling はそんなことはしなくなっていました。<br>現在の状況はもちろんこれとは違うんだろうし、望月に数学的内容を減らせとは言いません。けれど、肝となる発想がよくわからなくなっています。多分、彼に文章を **彩色**（グラフ理論的な意味で）してもらって、一般性を失うことなく、重要なステップがわかるようにしてもらうと良いのではないでしょうか？
      *  **Josh:** シンはすごい数学者だけれど、彼でさえどのステップが重要（特に、一般性が求められるのはどこか、特殊例でこと足りるのはどこか）というのはわかってないかもしれません。私が聞くところでは、彼は意図的に取っ付きづらいやりかたをしているということではないようです。
* **Edward R.:** ウェブサイトを見ればわかるよう、山下剛は何ヶ月もの間 "A proof of abc conjecture after Mochizuki" という論文を書き続けています。聞く所によれば、多分この論文は望月のあまりに作り込み過ぎた証明をすっきりさせて、分かり易い abc 予想の証明を与えてくれるのではないかと思います。ワークショップでは山下のこの論文について何かコメントはありましたか？作業は順調なのでしょうか？それと、星は「宇宙際 Teichmüller 理論入門」という 84 ページの論文を11月に出していますね。でも日本語です。この論文が英語に翻訳されるかもしれないという話はありましたか。 よろしくお願いします。
  *  **Brian Conrad:** Edward R. さん、山下は最低でも2年間、この論文を書き続けています。最初の目標はこの前の３月でした（最初の IUT 研究集会の時です）。オックスフォードでの集会での最初の講演で、彼はまだ書き続けていると言っていて、ページ数は「200ページ以上、だが間違いなく1000ページ以内」と言っていました（私の耳が間違えていなければ）。今のところオックスフォードの集会でのスライドがあるだけです。星のサーベイについては、星に翻訳の予定はあるかと尋ねましたが、ないとの答えでした。日本の慣習を私より知っている人の話では、彼より上の立場の人間が翻訳するということは有り得ないようです。なので、ワークショップの週が終わってから、かなり優秀な日本人院生（IUT論文を読み込んでいて、星のサーベイも読んだ院生）にアプローチして、翻訳できる見込みはあるかと尋ねました。しかし、この論文を翻訳するにはIUTをしっかり理解していないと無理だということで、できる人が思い付かないとの答えでした。これらのサーベイ論文について今私が把握していることは以上です。
  *  **Brian Conrad:** Edward R. さん：新しい情報です。星と直接話した人によれば、彼（星）が来夏の京都でのワークショップまでにサーベイを英訳したいと思っていると言っていたそうです。
