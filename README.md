# ceneoscraper
## Etap 1 Pobranie składowych pojedynczej opinii o konkretnym produkcie z serwisu \[Ceneo.pl](https://www.ceneo.pl/)
1. pobranie kodu pojedynczej strony z opinami o produkcie
2. Analizastrukturypojedyńczej kodu

|Składowa|Selektor CSS|Nazwa zmiennej|Typ danych|
|:-------|:----------|:----------|:-----------|
|Opinia|`div.js_product-review`|review||
|Identyfikator opinii|`[data-entry-id]`|review id||
|Autor opinii|`span.user-post__author-name|`|author||
|Rekomendacja|`span.user-post__author-name`|recommendation||
|Liczba gwiazdek|`span.user-post_score-count`|stars||
|Treść opinii|`div.user-post__text`|content||
|Lista zalet||||`div.review-feature__col:has(> div.review-feature__title--positives) > div.review-feature__item`
`div.review-feature__col:has(> div[class*="positives"]) > div.review-feature__item`
`div.review-feature__title--positives ~ div.review-feature__item|`
|Lista wad||||.review-feature_col|
|Dla ilu osób przyatna||||\votes-yes id|
|Dla ilu osób nieprzydatna|||||\votes-no id|
|Czy potwierdzona zakupem||||.review-pz|
|Data wystawienia opinii||||.user-post__publish|
|Data zakupu produktu||||.user-post__publish|

|Składowa|Selektor CSS|Nazwa zmiennej|Typ danych|
|:-------|:-------|:-------|:-------|
|Opinia|.user-post__cardtekst opinii||string|
|Identyfikator opinii|user-post__card[data-entry-id]||string|
|Autor opinii|.user-post__author-name||string|
|Rekomendacja|.user-post__author-recomendation||string|
|Liczba gwiazdek|.score-container||number|
|Treść Opinii|.user-post__text|||
|Lista zalet|.review-feature_col|||
|Lista wad|.review-feature_col|||
|Dla ile osób przydatna|\votes-yes id|||
|Dla ilu osób nieprzydatnych|\votes-no id|||
|Czy Potwierdzona zakupem|.review-pz|||
|Data wystawienia opinii|.user-post__publish|||
|Data zakupu produktu|.user-post__publish|||

div.review-feature__col:has(> div.review-feature__title--positives) > div.review-feature__item
div.review-feature__col:has(> div[class*="positives"]) > div.review-feature__item
div.review-feature__title--positives ~ div.review-feature__item

`span[id^="votes-no"]`<br>`button.vote-no["data-total-vote"]`<br>`button.vote-no > span`

