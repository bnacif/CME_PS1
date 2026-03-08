The goal of this project is to estimate the expected return of buying the cheapest ticket of Mega-Sena given an announced prize.
To do so, I use two primary data soucres. I describe them below.

    1. The first source is the file "Mega-Sena.xlsx", published by Caixa Econômica Federal on the website 
    "https://loterias.caixa.gov.br/Paginas/Mega-Sena.aspx" under the "Downloads" section. It details the 
    results of each draw of the lottery since 1996. Mainly, it reports the announced prize for each draw,
    the number of winners and the total revenue collected. To properly run the code, you must download the
    file and save it under `data/raw`.

    2. The second source informs the history of changes in the price of the cheapest ticket over the period
    of analysis. It needed to be constructed from independent announcements published in the Diário Oficial
    da União during this time. All files used for that are under the directory `others/price_changes`,
    including a text file with the original links for authentication. You do not need to reconstruct this dataset,
    as this is already handled by the code.

The code includes a function that deals with joining both datasets.

Besides the data aspects, the `output` folder contains the set of graph produced by the code. You must uncomment the `savefig` lines to store the plots in this folder.

**AI use**: I have used AI for learning purposes only. Specifically, I used Gemini and Claude to improve my knowledge of Julia programming, along with web research.
