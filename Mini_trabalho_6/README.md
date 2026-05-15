========================================================
  Mini Trabalho 6 — Otimização e Ajuste Fino
  Aprendizado de Máquina — UnB / FCTE
  Grupo 5
========================================================

MEMBROS:
  - Gustavo Costa de Jesus            (211061814)
  - Harleny Angéllica Araújo de Sousa (211061832)
  - João Pedro Araújo de Freitas Lyra (232003661)
  - Raquel Ferreira Andrade           (211062437)

--------------------------------------------------------
CONTEÚDO DO ARQUIVO ZIP:
--------------------------------------------------------
  mini_trabalho_6.ipynb                        → Notebook com otimização e ajuste fino
  README.txt                                   → Este arquivo
  dados_processados/ratings_processado.csv     → Dataset processado do Mini Trabalho 4
  assets/otimizacao_ncomponents.png            → Gráfico de RMSE por n_components
  assets/antes_depois.png                      → Comparação antes e depois da otimização

--------------------------------------------------------
DATASET UTILIZADO:
--------------------------------------------------------
  Dados processados gerados no Mini Trabalho 4, porém repetidos no 6
  Caminho esperado: ../Mini_trabalho_6/dados_processados/ratings_processado.csv

--------------------------------------------------------
COMO EXECUTAR:
--------------------------------------------------------
  1. Instale as dependências:
     pip install pandas numpy matplotlib scikit-learn

  2. Abra o notebook:
     jupyter notebook mini_trabalho_6.ipynb

  3. Execute: Kernel > Restart & Run All

--------------------------------------------------------
ETAPAS REALIZADAS:
--------------------------------------------------------
  1. Validação cruzada com 5 folds no SVD base (n_components=50)
  2. Otimização de hiperparâmetros testando n_components: 10, 20, 50, 100, 150
  3. Comparação do desempenho antes e depois da otimização