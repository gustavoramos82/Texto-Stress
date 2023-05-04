# Predição de Stress Humano

Neste projeto, será feito uma *análise de sentimentos* para avaliar se o texto apresenta o stress ou não, a partir de dataset obtido no *kaggle* (que pode ser obtido [aqui](https://www.kaggle.com/datasets/kreeshrajani/human-stress-prediction)) na qual foi extraido texto de comunidades no reddit.

Se quiser ler mais sobre o tema de **NLP** pode acessar o material no notion [aqui](https://flint-texture-e2f.notion.site/NLP-53af1cee1fed4ae8aaa70e8a77cc1a74) no qual está os materiais que estudei e os slides.

## Análise Exploratória

Foi escolhido do datset apenas três colunas, sendo elas:

- **Subreddit**: Comunidade de onde o texto foi retirado;
- **Texto**: Texto que será utilizado para detecção de stress;
- **label**: 1 se for pra stress, 0 caso contrário.

Se olharmos a quatidade de labels, veremos que os mesmo tem quase a mesma qualidade, ou seja, não há um desbalanceamento dos dados.

![image](https://user-images.githubusercontent.com/39843884/229916976-cb41e149-6150-4055-b34d-b29a63b38cbe.png)

Por comunidade, veremos que as comunidade que tem mais textos tem a ver com relações, ansiedade e ptsd (stress pós-traumático).

![image](https://user-images.githubusercontent.com/39843884/229917453-947c94e3-1d7d-4b50-89d6-e488d758f50c.png)

Separando as comunidades por label, temos que algumas comunidades apresentam mais textos como stress do que outras, como ansiedade e ptsd, que apresnetam mais textos com stress

![image](https://user-images.githubusercontent.com/39843884/229918220-6e5d7c39-8e10-4313-a8b9-3aa5ca06d5df.png)

- Comparando os wordclous entre textos com stress e sem, vemos que não há muito difrença nas palavras, apenas a palavra ansiedade que se tem no texto com stress.

Wordcloud do texto sem stress
![image](https://user-images.githubusercontent.com/39843884/229918857-e9624d71-132a-4af3-8f31-0ce5b606b07b.png)

Wordcloud do texto com stress
![image](https://user-images.githubusercontent.com/39843884/229919309-142d350b-6365-4b19-aeda-bf8c82d67890.png)

## Modelagem

Depois de um pré-processamento, foi dividido o dataset em 70% de treino e 30% de teste, da qual se utilizou vários algoritmos de machine learning, da qual se obteve os seguintes resultados.

(Se quiser entender um pouco mais sobre clique [aqui](https://github.com/gustavoramos82/Texto-Stress/blob/main/M%C3%A9tricas%20de%20Clasiifica%C3%A7%C3%A3o.md)).

![image](https://user-images.githubusercontent.com/39843884/229920628-d433cf17-cb14-4181-85af-bd2f7db65eb9.png)

## Consideraçẽs Finais

Comparando as métircas, podemos ver que:

- Comparando as métricas, podemos ver que os modelos com melhor perfomace foram  *Multinomial NB* (naive bayes), *SVM* com kernel sigmoid, e o *Catboost*.

- Poderia ser feito o metodo embbeding na tokenização;

- Fazer o cross-validation para comparar o resultado de vários testes.

![image](https://user-images.githubusercontent.com/39843884/233484847-7c15a251-c252-497d-a244-3b67e3ffc5e8.png)

- Fazer uma maior investigação pra ver se existem termos que tem mais uma classe do que outro.

