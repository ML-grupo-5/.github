# Modelagem e Avaliação — Sistema de Recomendação

Projeto da disciplina **Aprendizado de Máquina (UnB)** com foco na implementação e avaliação de modelos de recomendação de filmes.

---

## Integrantes

| Nome | Matrícula |
|------|----------|
| Gustavo Costa de Jesus | 211061814 |
| Harleny Angéllica Araújo de Sousa | 211061832 |
| João Pedro Araújo de Freitas Lyra | 232003661 |
| Raquel Ferreira Andrade | 211062437 |

---

## Base de Dados

Dados processados do MovieLens utilizados no Mini Trabalho anterior:

- `ratings_processado.csv`

Total:
- 90.274 avaliações

---

## Modelos Implementados

### 1. Baseline
- Predição utilizando a média global das avaliações

**RMSE:** `1.0275`

---

### 2. KNN
- Modelo baseado em similaridade entre usuários
- Utilização da métrica cosseno

**RMSE:** `1.0262`

---

### 3. SVD
- Fatoração de matriz com `TruncatedSVD`
- Redução de dimensionalidade da matriz usuário-filme

**RMSE:** `0.9886`

---

## Comparação dos Modelos

| Modelo | RMSE |
|--------|------|
| Baseline | 1.0275 |
| KNN | 1.0262 |
| SVD | **0.9886** |

Resultado:
- O modelo **SVD** apresentou o melhor desempenho.

---

## Conclusões

- O Baseline serviu como referência inicial.
- O KNN apresentou pouca melhoria devido à alta esparsidade dos dados.
- O SVD conseguiu capturar melhor os padrões de preferência dos usuários, obtendo o menor RMSE.

---

## Próximos Passos

- Ajuste de hiperparâmetros
- Testes com modelos híbridos
- Geração de recomendações personalizadas
- Avaliação com novas métricas

---

## Execução

No notebook Jupyter, rode:

```python
!pip install pandas numpy matplotlib scikit-learn scipy implicit
```

Depois execute as células do notebook normalmente.