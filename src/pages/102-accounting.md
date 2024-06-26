# 原価計算の考え方

## 人件費は原価か？販管費か？
  
粗利 ＝ 売上 ー 売上原価  
経常利益 ＝ 粗利 ー 販管費  
  
ですが、一般的に、人件費は固定費であり、販管費として扱われます。  

そのため、システム開発やWeb制作の会社は、会計上は売上原価ゼロ、粗利100％となることが多いです。  
  
そうなると、経常利益でしか会社の状態を図ることができず、  
プロジェクトの粗利率の低下が利益を圧迫したのか、販管費の増加が原因なのか、原因の切り分けが難しくなります。  
  
一方、人件費を売上原価としてしまうと、本来販管費である営業活動や社内業務、研修等の時間も原価に入ってしまい、やはり実態とかけ離れてしまいます。  
  
そこで、人件費を売上原価である直接労務費と、販管費である間接労務費に分解して考える、というのがヒト×ツキのベースとなる考え方です。  
  
実際の各スタッフの給与を時給換算したもの（またはその近似値）を労務費単価として登録することで、売上原価である労務費を正確に把握することができます。  
（社会保険料などは、あくまで販管費であるため、単価に含めません。）  
  
そして、実際の給与総額から、ヒト×ツキ上で算出された合計労務費を引いたものが、間接労務費（販管費）となります。  
  
## 売上原価の計算

売上原価＝労務費＋外注費＋諸経費  
  
ヒト×ツキでは、労務費のほか、外注費や諸経費も売上原価として入力できるようになっています。  

## OJTなどの扱い

OJT中の新人の労務費単価を、単純に給与の時給換算とすると、新人の関わったプロジェクトの粗利率が、実体より低くなってしまいます。  
  
OJT中の新人の場合、労務費単価は、単純時給の 1/2 〜 1/3 に設定することをお勧めします。  

例えば 1/3 に設定された新人が6時間作業した場合、  
2時間分は案件の稼働（売上原価）、4時間分は研修の時間（販管費）ということになり、実体に即した計算になります。  
