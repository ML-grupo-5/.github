## Recomendação de filmes

Este repositório é destinado ao projeto "Recomendação de filmes" da disciplina Aprendizado de Máquina, visando desenvolver um sistema de recomendação de filmes utilizando técnicas de Machine Learning. Para isso, foram coletados e analisados datasets públicos contendo avaliações de usuários sobre filmes.
Os dados serão utilizados para treinamento e validação de algoritmos capazes de recomendar filmes com base nas preferências dos usuários.

## Integrantes

| Nome | Matricula |
|------|-----------|
| Gustavo Costa de Jesus | 211061814 |
| Harleny Angéllica Araújo de Sousa | 211061832 |
| João Pedro Araújo de Freitas Lyra | 232003661 |
| Raquel Ferreira Andrade | 211062437 |

## Bases de dados

Serão utilizados datasets da coleção MovieLens, disponibilizados pelo GroupLens Research:
- MovieLens 100K
https://grouplens.org/datasets/movielens/latest/
Utilizado para testes iniciais, validação e experimentação dos algoritmos.
- MovieLens 32M
https://grouplens.org/datasets/movielens/32m/
Utilizado para o treinamento principal do modelo, pois contém cerca de 32 milhões de avaliações, permitindo maior precisão nas recomendações.

Embora os datasets utilizados sejam públicos, a aplicação considera boas práticas de segurança para dados de usuários. Entre as medidas adotadas estão:
- Isolamento do banco de dados em rede interna utilizando Docker;
- Uso de criptografia para dados armazenados e em trânsito (HTTPS/TLS);
- Pseudonimização de dados pessoais;
- Envio apenas de dados genéricos para a IA;
- Transparência e possibilidade de exclusão de dados pelo usuário.

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
