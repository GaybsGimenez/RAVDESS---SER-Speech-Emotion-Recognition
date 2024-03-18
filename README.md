# Reconhecimento de Emoções na Fala - RAVDESS

Este notebook explora como entender as emoções transmitidas pela fala usando a base de dados RAVDESS.

## O Que é RAVDESS?

RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song) é um conjunto de dados com mais de 7000 arquivos de áudio gravados por 24 atores profissionais. Eles expressam diferentes emoções, como felicidade, tristeza, raiva e medo.

## Objetivo

Vamos treinar um modelo de aprendizado profundo para identificar automaticamente as emoções em arquivos de áudio.

## Passos Principais:

1. **Importação de Bibliotecas e Dados:** Aqui, carregamos as ferramentas necessárias e baixamos os arquivos de áudio.
  
2. **Análise dos Dados:** Damos uma olhada rápida nos dados para entender como as emoções estão distribuídas.

3. **Pré-processamento:** Preparamos os dados, extraindo recursos importantes como os MFCCs (Mel-frequency cepstral coefficients).

4. **Treinamento do Modelo:** Criamos e treinamos uma rede neural para aprender a reconhecer as emoções na fala.

5. **Avaliação do Modelo:** Testamos o modelo em dados de teste para ver quão bem ele está performando.

6. **Teste em Novos Dados:** Finalmente, usamos o modelo para prever emoções em novos arquivos de áudio e vemos como ele se sai.


## Introdução

A base de dados RAVDESS é composta por 7356 arquivos de áudio, totalizando 24,8 GB. Esses arquivos incluem gravações de 24 atores profissionais (12 mulheres e 12 homens), vocalizando declarações lexicalmente combinadas em um sotaque norte-americano neutro, representando várias emoções, como calma, felicidade, tristeza, raiva, medo, surpresa e desgosto.

## Importando Bibliotecas e Dados

O notebook começa importando bibliotecas essenciais, como Pandas, Librosa e TensorFlow, para análise de dados e treinamento de modelos de aprendizado profundo. Em seguida, os conjuntos de dados de áudio são baixados e extraídos.

## Análise Exploratória de Dados (EDA)

Após a importação dos dados, são realizadas análises exploratórias para entender a distribuição das emoções nos arquivos de áudio. Isso inclui visualizações de formas de onda, espectrogramas de STFT e MFCCs (Mel-frequency cepstral coefficients).

## Pré-processamento

Os arquivos de áudio são pré-processados para extrair recursos relevantes, como os MFCCs. Os dados são divididos em conjuntos de treinamento e teste, e as etiquetas são codificadas em one-hot vectors.

## Treinamento do Modelo

Um modelo de Rede Neural Convolucional (CNN) é criado e treinado com os dados de treinamento. O treinamento é monitorado usando dados de validação e checkpoints são salvos para o melhor modelo.

## Avaliação do Modelo

O modelo treinado é avaliado usando os dados de teste para medir sua precisão e perda. Visualizações são fornecidas para entender o desempenho do modelo.

## Teste em Novos Dados

Por fim, o modelo é testado em novos arquivos de áudio para prever as emoções presentes neles. Uma análise detalhada é fornecida, incluindo visualizações de forma de onda e espectrogramas, juntamente com as emoções previstas.

Espera-se que este notebook ajude na compreensão e implementação do reconhecimento de emoções na fala utilizando aprendizado profundo, com foco na base de dados RAVDESS.
