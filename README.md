# 🎯 Mega-Sena com Machine Learning

Este projeto aplica técnicas de **Machine Learning** sobre o histórico de sorteios da **Mega-Sena**, utilizando um dataset em formato CSV, com o objetivo de **analisar padrões estatísticos** e gerar um **ranking probabilístico dos números mais recorrentes**.

> ⚠️ Importante: a Mega-Sena é um processo aleatório.  
> Este projeto **não prevê resultados futuros**, apenas realiza **análise estatística baseada em dados históricos**.

---

## 📌 Objetivo do Projeto

- Aplicar **Machine Learning de forma correta** em um problema de loteria
- Evitar erros conceituais comuns (uso de índice do sorteio, ordem das bolas, etc.)
- Gerar:
  - Ranking de números mais prováveis
  - Melhor jogo sugerido
  - Múltiplos jogos baseados no histórico

---

## 🧠 Abordagem Utilizada

O problema foi modelado como uma **classificação multilabel**, onde:

- Cada sorteio é convertido em um **vetor binário de 60 posições**
- `1` indica que o número foi sorteado
- `0` indica que o número não foi sorteado

O algoritmo escolhido foi o **Random Forest Classifier**, por sua capacidade de capturar padrões estatísticos e relações não lineares.

---

## 🗂️ Estrutura do Dataset

O dataset deve estar no formato CSV e conter as seguintes colunas:

- `Ball1`
- `Ball2`
- `Ball3`
- `Ball4`
- `Ball5`
- `Ball6`

Cada linha representa um sorteio da Mega-Sena.

Exemplo:

```csv
Ball1,Ball2,Ball3,Ball4,Ball5,Ball6
5,12,23,34,45,56
1,9,18,27,36,42
