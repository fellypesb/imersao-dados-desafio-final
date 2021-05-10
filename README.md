
# Projeto Data Science: *Machine learning* aplicado em *Drug discovery*

![image](https://user-images.githubusercontent.com/52214785/117591833-8f7d2780-b10c-11eb-9df5-05844ec1c169.png)


Este repositório contém um simples projeto de *Data Science* desenvolvido durante a terceira edição do #imersão_dados realizado pela alura. O projeto foi realizado utilizando a linguagem *python* e diversas bibliotecas específicas da área de *Data Science* e *Machine Learning*, sendo as principais:

+ Pandas - Para importação e exploração dos dados;
+ Seaborn - Para visualização dos dados;
+ Scikit-Learn - Para construção dos modelos preditivos.

A área de estudo explorado, foi o *Drug discovery* que consiste na descoberta de novos fármacos por meio de pesquisas científicas. No entanto, o trabalho que antes era manual, agora está sendo revolucionado graças a biotecnologia e diversas ferramentas computacionais que contribuem de forma significativa para construção e descoberta de novos compostos. Está área, também envolve massivas quantidade dados gerados durantes os experimentos e, nesse contexto, a ciência de dados surge como grande aliado no desenvolvimento da farmacologia.

# Objetivo

Este projeto teve como objetivo a aplicação de técnicas de *Data Science* na descoberta de novos farmácos. Além disso, verificar a possibilidade de criação de um modelo preditivo capaz de descobrir ou auxiliar na descoberta desses fármacos de forma mais rápida e eficiente.

# Estrutura dos dados

Os dados foram estruturados no formato [*tidy*](https://escoladedados.org/tutoriais/tidy-data-dados-arrumados-e-5-problemas-comuns/), isto é, de forma que cada coluna representa os atributos da base dados e cada linha representa uma amostra dos resultados obtidos para cada composto testado.

Os atributos explorados na base de dados foram:

+ Tipo de tratamento do experimentos;
+ Tempo de análise das reações aos compostos testados;
+ Compostos utilizados;
+ E diversas expressões gênicas.

# Metodologia

A metodologia abordada trata-se das principais etapas de um projeto de *Data Science*. Inicialmente foi realizado uma análise inicial dos dados (AED) com o simples objetivo de obter  *insights* dos dados. Em seguida, foi realizada uma breve e superfícial análise estatística dos principais atributos para coleta de informações mais detalhadas e precisas. E ao final, sintetizando todas as informações obtidas, iniciou-se a fase de prototipagem dos modelos preditivos. Testou-se alguns diferentes modelos até alcançar o modelo mais preciso.

# Resultados

Para alcançar o mehor modelo preditivo utilizou-se a técnica de otimização de hiperparâmetros com o auxílio do algoritmo *Randomized Search*. O modelo escolhido foi o *Multilayer perceptron* (MLP), baseado em redes neurais artificias. A escolha desse modelo foi motivada por interesses pessoas de estudo e pela crecente aplicação, com sucesso, das redes neurais artificias, nas mais variadas áreas do conhecimento humano. O melhor modelo MLP treinado possue as seguintes configurações:

+ Número de neurônios na camada oculta = 8
+ Tipo de aprendizado = 'invscaling'
+ Taxa de aprendizado inicial = 0,5358867312681471
+ Constante de momento = 0.04927989038222336
+ Tamanho dos lotes = 16
+ Constante alfa de regularização = 0,1
+ Quantidade de atributos preditores = 872

Com estas configurações foi possível obter uma pontuação de aproximadamente 65% no conjunto de teste. É Importante ressaltar que em todos os processos que utilizaram sementes de valores aleatórios, utilizou-se a semente 42. Dessa forma, é possivel garantir a reprodutibilidade dos resultados em qualquer máquina, local e horário.

# Conclusões

Ao analisar os resultados dos modelos preditivos foi possível perceber que os modelos desevolvidos obtiveram apenas acurácias razoáveis próximo de 50% de precisão, mesmo após aplicar otimização nos hiperparâmetros do modelo. No entanto, a área de *Drug Discover* necessita de precisões mais altas principalmente por se tratar de compostos que poderão ser distribuídos a pessoas no tratamento de alguma doença. Portanto, conclui-se que é necessário mais estudos e aprimoramento das técnicas utilzadas para que possa de fato contribuir no descobrimento de novos compostos de forma mais precisa.

## Sugestão de trabalhos futuros
Como sugestão de trabalhos futuros propoẽm-se reduzir a dimensionalidade do modelo preditivo (quantidade de atributos de entrada), selecionando apenas os atributos mais importantes para o modelo e excluindo os demais, solucionando possíveis problemas com a chamada **maldição da dimensionalidade**.

## Agradecimentos
Agradeço a todo time da alura que proporcionou uma semana íncrivel de muito *Data Science* na imersão dados ❤️  

Em especial, agradeço os professores dessa edição:  

Thiago Santos  
Guilherme Silveira  
Vanessa Leiko  

## Referências

**Documentação:** [pandas](https://pandas.pydata.org/docs/)  
**Documentação:** [scikit-learn](https://scikit-learn.org/stable/index.html)  
**Livro:** [Machine Learning](https://www.amazon.com.br/Machine-Learning-Refer%C3%AAncia-Trabalhando-Estruturados/dp/857522817X)  
**Fundamentação teórica:**[Drug Discover](https://en.wikipedia.org/wiki/Drug_discovery)


