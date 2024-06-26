# 案件タイプの仕様

案件には、以下の4つのタイプがあります。

- 単発売上
- 継続売上
- 工数比例売上
- 営業外

違いは主に、売上の計算方法です。

## 単発売上

毎月進捗率を入力することにより、売上が計上されます。  

典型的には、納品まで数ヶ月以上かかるような、新規開発案件です。  
要件定義、設計、製造、結合テストといった「フェーズ」を登録することができ、フェーズごとの見積額と進捗率を登録できます。  
  
小規模なスポット案件も、単発売上タイプで登録することになります。  

## 継続売上

毎月決まった売上が自動的に計上されます。  
特定月の売上のみを変更することも可能です。  
  
典型的には、保守契約のように、毎月一定額を請求する案件です。

## 工数比例売上

日報に入力された工数✕請求単価 で自動的に売上が計上されます。  
請求単価は案件ごとに固定です。  
  
いわゆる準委任案件がこれにあたります。  
  
このタイプを選択した場合、日報入力時に「作業時間」と「請求時間」の2つの入力欄が有効になります。  
通常この2つの欄には同じ値を入力しますが、
例えば社内での引継ぎ作業など、稼働はしている（原価にはなる）が、お客様には請求できない時間は、請求時間を 0 とすることで、売上金額に反映しないことができます。  
作業明細には稼働時間ではなく請求時間が表示され、請求時間が 0 の明細は表示されません。  

### SESの扱いについて

「工数比例売上」タイプは作業者ごとに請求単価を変えることができないため、人によって単価が異なる場合、人ごとに案件を登録することになります。  
  
また、期間によって請求単価を変更することができないため、単価の見直しがあった場合、新たに案件を登録する必要があります。  

例えば、月140〜160時間までは月80万円、140時間を切ったら減額、160時間を切ったら加算・・・といったような契約には対応しておりませんので、  
こういうケースでは、「継続売上」の方が向いているかもしれません。  
  
※ SES案件を想定した新たな案件タイプ、もしくは工数比例売上タイプの機能追加を検討中です。  

## 営業外

売上（納品）に直接繋がらない社内業務や研修、営業活動などは、「営業外」として登録します。  
「営業外」タイプの案件は、稼働時間の集計はされますが、収支計算に反映されます。  
