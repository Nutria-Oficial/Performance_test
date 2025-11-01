# Performance_test: Análise de Teste A/B de Usabilidade

Este repositório contém o Jupyter Notebook (`main.ipynb`) e os dados de análise de um teste A/B realizado para comparar dois fluxos de usuário (A e B) em um aplicativo.

O objetivo da análise é determinar, com significância estatística, qual fluxo proporciona a melhor performance, medido pelo tempo de conclusão da tarefa.

## 🎯 Hipótese

Nossa hipótese era que o **Fluxo B**, com menos telas, uma paleta de cores ajustada e botões reorganizados, resultaria em uma redução estatisticamente significativa no tempo médio de conclusão da tarefa.

## 🧪 O Teste: Fluxo A vs. Fluxo B

* **Fluxo A (Controle):** O design original da aplicação.
* **Fluxo B (Variante):** O novo design, que implementou as seguintes mudanças:
    * **Redução no número de telas:** Para diminuir a insegurança e aumentar a confiança.
    * **Ajuste na paleta de cores:** Tom de laranja escurecido para maior conforto visual.
    * **Reorganização de botões:** Para um fluxo de navegação mais lógico.

## 🚀 Como Replicar a Análise

O notebook `main.ipynb` contém todo o cálculo estatístico (Teste Z) usado para validar os resultados.

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/Nutria-Oficial/Performance_test.git](https://github.com/Nutria-Oficial/Performance_test.git)
    cd Performance_test
    ```

2.  **Instale as dependências:**
    O notebook utiliza a biblioteca `scipy` para os cálculos estatísticos.
    ```bash
    pip install scipy
    ```

3.  **Execute o Jupyter Notebook:**
    Abra o arquivo `main.ipynb` em um ambiente Jupyter (como Jupyter Lab ou VS Code) e execute as células. O notebook é interativo e permite calcular a significância para diferentes intervalos de confiança.

## 📈 Conclusão e Decisão

**Decisão: O Teste B é o vencedor.**

A análise estatística, realizada com um **intervalo de confiança de 95%**, confirmou que a diferença entre os grupos é estatisticamente significativa.

* **Fluxo A (Controle):** Tempo médio de 52.09 segundos.
* **Fluxo B (Variante):** Tempo médio de 42.87 segundos.

Isso representa uma **redução de aproximadamente 17,7%** no tempo médio de conclusão, validando nossa hipótese. Recomendamos a implementação do Fluxo B para 100% dos usuários.

## 📊 Relatórios de Coleta de Dados (Maze)

Os dados brutos para esta análise foram coletados através da plataforma Maze.

* **Relatório Teste A:** `https://app.maze.co/report/Teste-A/1js3o7mgf6t83a/intro`
* **Relatório Teste B:** `https://app.maze.co/report/Teste-B/1siu7mgv7n5hx/intro` 
