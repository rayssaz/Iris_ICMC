# Aplicação de modelos de classificação utilizando o dataset Iris
 ## Sobre o Dataset
 O dataset Iris é um dos conjuntos de dados mais conhecidos e amplamente utilizados em
 machine learning e estatística, especialmente para problemas de classificação. Ele foi
 coletado por Ronald A. Fisher em 1936 e contém informações sobre três espécies de flores
 do gênero Iris:
 * Iris setosa
 * Iris versicolor
 * Iris virginica
 
 O dataset contém 150 amostras, divididas igualmente entre as três espécies de flores (50
 amostras por espécie). Cada amostra possui 4 características medidas em centímetros, que
 representam aspectos morfológicos das flores. Essas características são:
 
 * SepalLengthCm: Comprimento da sépala
 * SepalWidthCm: Largura da sépala
 * PetalLengthCm: Comprimento da pétala
 * PetalWidthCm: Largura da pétala
   
 Além dessas características, o dataset contém uma coluna chamada Species, que é o alvo
 de classificação e indica a espécie de cada flor.

## Objetivo 
Projetar e analisar os modelos de aprendizado de máquina criados para identificar corretamente a espécie de flor na base das características observadas da sépala e da pétala.

## Etapas
* Pré- processamento dos dados;
* Aplicação de métodos de classificação;
* Avaliação do desempenho do modelo gerado.

## Modelos utilizados 
### 1. Suporte ao algoritmo de aprendizado de máquina vetorial (SVM):

O Support Vector Machine (SVM) é um algoritmo de aprendizado de máquina supervisionado. Resolve problemas envolvendo classificação e regressão. No SVM, os dados são divididos em classes separadas por um hiperplano (uma linha). O SVM visa localizar o hiperplano que maximiza a distância entre classes distintas, um processo conhecido como maximização de margem, o que aumenta a probabilidade de classificar corretamente os dados. A previsão do mercado de ações é uma das aplicações do SVM.

### 2. K-Nearest Neighbors (KNN):
O algoritmo K-Nearest Neighbors (KNN) é um classificador de aprendizado supervisionado não paramétrico, que usa a proximidade para fazer classificações ou previsões sobre o agrupamento de um ponto de dados individual. É um dos classificadores de classificação e regressão populares e mais simples usados no aprendizado de máquina hoje.

## Métricas 
### Acurácia: Proporção de exemplos que foram preditos corretamente pelo modelo.
### Precisão: Identifica quais exemplos que o modelo classificou como positivo, realmente eram positivos.
### Recall (sensibilidade): Avalia quantos exemplos da classe positiva o modelo acertou. Usado quando os falsos negativos forem mais importantes que os falsos positivos.
### F1-score: Combina precisão e recall em uma métrica única que indique a qualidade geral do modelo. É calculada a partir da média harmonica entre precisão e recall.

2 *  (Precisão * Recall / Precisão + Recall)

# Análise dos modelos
No caso do modelo SVM, verificamos através da matriz de confusão que houve um caso de Falso Positivo. Um exemplo foi classificado como positivo, sendo Iris versicolor, no entanto, o exemplo era Iris virginica.

![image](https://github.com/user-attachments/assets/6e051df7-5f16-406a-bad8-2f5b3bd5dbf9)

O modelo de SVM obteve acurácia 0.97, enquanto o modelo KNN obteve o valor 1.0, identificando corretamente todos os exemplos avaliados. 

![image](https://github.com/user-attachments/assets/f6a6d0fb-5704-45c8-9035-29c52caa54ec)

De modo geral, ambos os modelos tiveram valores altos, sendo bons classificadores para esse dataset.
