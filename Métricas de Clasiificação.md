## Sobre as métricas de classificação

A fonte para essa explicação pode ser acessado [aqui](https://medium.com/kunumi/m%C3%A9tricas-de-avalia%C3%A7%C3%A3o-em-machine-learning-classifica%C3%A7%C3%A3o-49340dcdb198).

As métricas de clasicação são obtidas a partir da matriz de confusão, que permite visualizar facilmente quantos exemplos foram classificados corretamente e erroneamente em cada classe, ajudando a entender se o modelo está favorecendo uma classe em detrimento da outra.

![image](https://camo.githubusercontent.com/15cb5abf76184b9d2ee730802fe72e36fd824553aee195d1b6e0e053a41ff997/68747470733a2f2f757365722d696d616765732e67697468756275736572636f6e74656e742e636f6d2f33393834333838342f3233333437393434322d63613439396665382d383730312d343838352d616166392d3039656661313038313438612e706e67)

![image](https://user-images.githubusercontent.com/39843884/236320938-e8cf0abf-068a-4d6a-aa51-a73100f7ac05.png)

- **Precisão**: Esta métrica é definida pela razão entre a quantidade de exemplos classificados corretamente como positivos e o total de exemplos classificados como positivos.

  
  

![image](https://user-images.githubusercontent.com/39843884/233481000-ef813924-e9fd-460b-b81b-fef58f463aee.png)

  

- **Recall**: Também chamdo de Revocação ,dá maior ênfase para os erros por falso negativo. Esta métrica é definida pela razão entre a quantidade de exemplos classificados corretamente como positivos e a quantidade de exemplos que são de fato positivos.

  

![image](https://user-images.githubusercontent.com/39843884/233481646-43deaaa7-5fc7-406b-b445-f2e910b3b0a3.png)
- **F1-Score**: Leva em consideração tanto a precisão quanto a revocação. Ela é definida pela média harmônica entre as duas.Se a precisão ou a revocação for zero ou muito próximos disso, o F1-score também será baixo. Desta forma, para que o F1-score seja alto, tanto a precisão como a revocação também devem ser altas.

  
  ![image](https://user-images.githubusercontent.com/39843884/233481977-1e82a022-badb-4152-9a6d-ff0f390443eb.png)
