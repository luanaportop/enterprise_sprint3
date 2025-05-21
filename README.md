# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href="https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Administração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Enterprise Challenge - Sprint 3

## Beginner Coders

## 👨‍🎓 Integrantes:
- <a href="https://www.linkedin.com/in/luana-porto-pereira-gomes/">Luana Porto Pereira Gomes</a>
- <a href="https://www.linkedin.com/in/luma-x">Luma Oliveira</a>
- <a href="https://www.linkedin.com/in/priscilla-oliveira-023007333/">Priscilla Oliveira </a>
- <a href="https://www.linkedin.com/in/paulobernardesqs?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app">Paulo Bernardes</a>

## 👩‍🏫 Professores:
### Tutor(a)
- <a href="https://www.linkedin.com/in/leonardoorabona/">Leonardo Ruiz</a>
### Coordenador(a)
- <a href="https://www.linkedin.com/in/profandregodoi/">André Godoi</a>

## 📜 Descrição

Este projeto tem como objetivo realizar a **validação prática** do modelo de Inteligência Artificial desenvolvido na Sprint 2, 
correlacionando as previsões de produtividade agrícola da soja, realizadas com base no NDVI, com dados reais históricos obtidos de bases públicas.

## 📝 Sobre o Projeto

Foram utilizados três tipos principais de dados:

- **NDVI médio da safra**: obtido do sistema SATVeg da Embrapa.
- **Produtividade agrícola (rendimento médio)**: obtido do sistema IBGE/SIDRA.
- **Dados climáticos**: precipitação, temperatura e umidade média da safra, obtidos de bases públicas (INMET).

O trabalho foi desenvolvido como parte da Sprint 3 do Enterprise Challenge da FIAP, no 2º semestre do curso de Inteligência Artificial.

## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>assets</b>: arquivos relacionados a elementos não-estruturados deste repositório, como imagens.

- <b>dados</b>: aqui estão os dados utilizados no notebook, incluindo a base consolidada com NDVI, produtividade e clima.

- <b>notebook</b>: aqui está o download do notebook em .ipynb.

- <b>README.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

## 🔧 Como executar o código
### 🐍 Código Python:
   - Executar por meio do link do notebook: [coloque o link do Colab ou GitHub Pages aqui]
   - Faça upload do arquivo de dados `.xlsx`.
   - Execute as células do notebook em sequência.

## ⚙️ Etapas Realizadas

**1. Coleta e Organização dos Dados:**
- Coletamos séries históricas de NDVI usando o SATVeg.
- Coletamos dados oficiais de produtividade da soja no IBGE/SIDRA.
- Coletamos dados climáticos do INMET: precipitação, temperatura máxima e mínima, e umidade relativa.
- Juntamos todas as informações em uma **base consolidada** para análise.

**2. Análise Estatística:**
- Aplicamos correlação de **Pearson** e **Spearman** para avaliar a relação entre NDVI, variáveis climáticas e produtividade.
- Utilizamos também a **Informação Mútua** como métrica adicional.

**3. Modelagem de Regressão:**
- Realizamos regressão linear simples entre NDVI e produtividade.
- Realizamos regressões adicionais com variáveis climáticas como preditores.
- Aplicamos regressão linear múltipla combinando NDVI e variáveis climáticas para melhorar a explicação da produtividade.

**4. Visualização:**
- Foram gerados gráficos de dispersão com linha de tendência para todas as regressões.
- Realizamos gráficos comparativos entre variáveis.

**5. Discussão Crítica:**
- Analisamos a qualidade preditiva do NDVI e das variáveis climáticas.
- Apontamos limitações e sugerimos melhorias para o modelo.

## 📊 Principais Resultados

- A regressão linear simples entre **NDVI e produtividade** apresentou um R² de **0,0276**, indicando **fraca capacidade preditiva**.
- A variável climática com maior poder explicativo foi a **temperatura máxima**, com R² de **0,3033**.
- A regressão linear múltipla combinando NDVI e clima resultou em um R² de aproximadamente **0,41**, melhorando a capacidade de previsão.

Esses resultados indicam que o **NDVI isolado não é suficiente**, mas combinado com variáveis climáticas melhora a explicação da produtividade agrícola.

## 🧠 Conclusão

A análise demonstrou que o NDVI, quando utilizado em conjunto com variáveis climáticas, melhora a previsão de produtividade agrícola, mas ainda assim possui limitações.  
Para aprimorar o modelo, recomenda-se:
- Expandir a base de dados.
- Incorporar outras variáveis, como tipo de solo e manejo agrícola.
- Testar modelos não lineares.

## 🛠️ Tecnologias Utilizadas
- Python 3.11
- Google Colab
- Pandas
- Scikit-learn
- Matplotlib
- SATVeg (Embrapa)
- IBGE/SIDRA
- INMET

## 🗃 Histórico de lançamentos

* 0.5.0 - XX/XX/2024
    * Entrega final da Sprint 3.
* 0.4.0 - XX/XX/2024
    * Finalização da regressão linear múltipla.
* 0.3.0 - XX/XX/2024
    * Correlações estatísticas concluídas.
* 0*
