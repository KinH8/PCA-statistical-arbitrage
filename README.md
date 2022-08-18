# PCA-statistical-arbitrage
We will be implementing a PCA statistical arbitrage strategy on blue chip Malaysian equities as per Avellaneda and Lee (2008) Statistical Arbitrage in the US Equity Market, available at https://math.nyu.edu/~avellane/AvellanedaLeeStatArb20090616.pdf.

We first calculate each stock's idiosyncratic returns by backing out returns attributed to the top 15 principal components. We then select stocks with faster speed of mean reversion based on Ornstein-Uhlenbeck process. The 3rd step involves calculating the Z-score of each remaining stocks and allocate accordingly (i.e. overweight stocks with low Z-score relative to its historical Z-score).

Our portfolio is long-only due to short selling constraints in Malaysia, which differs from Avellaneda and Lee's long-short portfolio. Although annual return and Sharpe is high at 10.2% and 0.82, note that returns displayed are gross of costs. Sizing is naive at equal weighting so portfolio may be heavily concentrated in some positions if only few stocks are selected.

Credit: https://github.com/YuxiLiuAsana/Statistical-Arbitrage-Avellaneda-

![image](https://user-images.githubusercontent.com/105033135/185328156-4bfd4249-b762-4fde-919e-1fe78a04e276.png)

![image](https://user-images.githubusercontent.com/105033135/185328477-99c719fb-ba75-48b7-93ce-a6055e0529fd.png)

![image](https://user-images.githubusercontent.com/105033135/185331171-74d06440-2447-4934-9990-8880c19e3d8a.png)


