# brazil-railway-accident-forecasting
End-to-end data analysis of Brazilian railway accidents, from data cleaning and visualization to SARIMA forecasting.

# 📊 Análise e Projeção de Acidentes Ferroviários no Brasil

Este repositório contém um projeto completo de análise de dados sobre acidentes ferroviários no Brasil, utilizando dados públicos da Agência Nacional de Transportes Terrestres (ANTT) de 2004 a 2024. O projeto abrange todo o ciclo de vida da análise: desde a limpeza e preparação dos dados até a construção de um modelo de projeção com Séries Temporais (SARIMA).

O notebook principal (`Projeto2.ipynb`) documenta cada passo do processo, tornando a análise transparente e replicável.

---

## 🎯 Principais Insights da Análise

*   **Qualidade dos Dados:** Um desafio inicial foi a padronização da coluna `perimetro_urbano`, que revelou um insight crucial: a esmagadora maioria dos acidentes (**99.8%**) ocorre fora de áreas urbanas.

*   **Tipos de Acidentes Mais Comuns:** A análise demonstrou que três tipos de acidentes são predominantes: **Descarrilamento** (4.974 casos), **Atropelamento** (4.138 casos) e **Abalroamento** (4.125 casos).

*   **Volume vs. Gravidade:** Foi identificada uma diferença notável entre o volume de acidentes e a gravidade (fatalidades) por concessionária. A **MRS Logística** é a terceira em número de acidentes, mas a **primeira em número de óbitos**, indicando uma maior severidade em seus incidentes.

*   **Tendência Temporal:** O número de acidentes apresentou um pico significativo entre 2010 e 2015, seguido por uma estabilização em um patamar mais baixo nos anos subsequentes.

*   **Projeção Futura:** O modelo de forecasting (SARIMA) projeta uma leve tendência de queda para os próximos dois anos. No entanto, o amplo intervalo de confiança sugere uma alta incerteza, o que é esperado para séries temporais com dados anuais.

---

## 🛠️ Tecnologias Utilizadas

*   **Linguagem:** Python 3
*   **Bibliotecas de Análise:** Pandas, NumPy
*   **Bibliotecas de Visualização:** Matplotlib, Seaborn
*   **Bibliotecas de Modelagem:** Statsmodels (para o modelo SARIMA), Holidays
*   **Ambiente:** Jupyter Notebook

---

## 📂 Estrutura do Repositório

O projeto está organizado da seguinte forma para garantir clareza e reprodutibilidade:

```
├── data/
│   └── dataset.json         # Conjunto de dados original em formato JSON
│
├── notebooks/
│   └── Projeto2.ipynb       # Notebook principal com toda a análise
│
├── LICENSE                  # Licença do projeto (MIT)
└── README.md                # Este arquivo
```

---

## 🚀 Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/campagnoli/brazil-railway-accident-forecasting
    cd brazil-railway-accident-forecasting
    ```

2.  **Instale as dependências:**
    Certifique-se de que você tem todas as bibliotecas listadas na seção "Tecnologias Utilizadas" instaladas em seu ambiente Python.
    ```bash
    pip install pandas numpy matplotlib seaborn statsmodels holidays jupyter
    ```

3.  **Execute o Jupyter Notebook:**
    Abra e execute o notebook localizado em `notebooks/Projeto2.ipynb`.

    **Atenção:** O caminho para o arquivo de dados dentro do notebook está configurado como `../data/dataset.json`, de acordo com a estrutura de diretórios do projeto.

---

## 📄 Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).

---
