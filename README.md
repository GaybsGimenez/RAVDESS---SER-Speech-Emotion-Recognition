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
