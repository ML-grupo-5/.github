# Preparação dos Dados — MovieLens

Projeto da disciplina **Aprendizado de Máquina (UnB)** com foco em **pré-processamento de dados** para sistemas de recomendação.

---

##  Integrantes

| Nome | Matrícula |
|------|----------|
| Gustavo Costa de Jesus | 211061814 |
| Harleny Angéllica Araújo de Sousa | 211061832 |
| João Pedro Araújo de Freitas Lyra | 232003661 |
| Raquel Ferreira Andrade | 211062437 |

---

##  Base de Dados

- [MovieLens Latest Smal](https://grouplens.org/datasets/movielens/latest/)  
- 100.836 avaliações  

Arquivos utilizados:
- `ratings.csv`
- `movies.csv`

---

##  Etapas de Preparação

### 1. Limpeza e Filtragem
- Remoção de filmes com menos de **5 avaliações**
- Dataset reduzido: **100.836 → 90.274 avaliações**

---

### 2. Codificação de Gêneros
- Transformação da coluna `genres` em variáveis binárias (one-hot encoding)
- Resultado: **21 colunas de gêneros**

---

### 3. Normalização das Notas
- Centralização por usuário:
  - `rating_norm = rating - média do usuário`
- Escalonamento com **MinMaxScaler**:
  - `rating_scaled ∈ [0,1]`

---

### 4. Exportação
Arquivos gerados:

- `dados_processados/ratings_processado.csv`
- `dados_processados/movies_processado.csv`

---

##  Resultados

- Redução de ruído com filtragem de dados  
- Gêneros convertidos para formato numérico  
- Correção de viés individual dos usuários  
- Dados prontos para modelagem  

---

##  Execução

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
python script.py
