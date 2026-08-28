# 🎮 Steam Store Games Analysis Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen?style=for-the-badge)

Projeto de análise de dados desenvolvido durante a trilha de **Power BI da Fundação Bradesco**, aplicando conceitos de Business Intelligence para explorar o mercado de jogos digitais da Steam.

---

## 📈 Dashboard

![Dashboard Power BI](img/steam_dashboard.gif)

O dashboard permite filtragem por gênero, ano de lançamento e faixa de preço, oferecendo uma visão dinâmica do mercado.

### Principais Métricas

| Métrica | Valor |
|---|---|
| Total de jogos analisados | 27.000+ |
| Gênero mais incidente | Indie |
| Tag mais incidente | Puzzle |
| Faixa de preço dominante | R$10–R$60 |
| Menor preço médio (ano) | 2018 |

### 💡 Principais Insights

1. **Variação de Preço (2015–2018):** observou-se uma queda progressiva no preço médio dos jogos digitais neste período, atingindo o ponto mais baixo em 2018. Após essa data, houve uma tendência de alta (possível reflexo de mudanças cambiais e da indústria — hipótese não confirmada diretamente pelos dados).
2. **Dominância Indie:** a grande concentração de jogos está na faixa de **R$10 a R$60**, refletindo a predominância de jogos do gênero *Indie* na Steam, que possuem custos de produção e venda mais acessíveis.
3. **Uso de Tags:** a maioria dos jogos não utiliza tags descritivas detalhadas, limitando-se às categorias genéricas de gênero.

---

## 🎯 Pergunta Norteadora

A análise foi guiada pela seguinte questão:

> **"O que define a popularidade de um jogo? E como o gênero influencia nisso?"**

---

## 🧠 Metodologia e Métricas

Para responder à pergunta norteadora, foi necessário criar métricas que fossem justas entre diferentes gêneros de jogos.

### Métrica de Popularidade e Engajamento

Adotou-se a relação entre **Avaliações Positivas** e **Engajamento**. O Engajamento foi calculado combinando:

1. **Tempo de Jogo Médio** (Average Playtime)
2. **Mediana do Tempo de Jogo por Gênero** — para evitar que gêneros com jogadores "hiper focados" (como MMOs) distorcessem a análise global, ofuscando jogos narrativos ou casuais.

### Tratamento de Tags

Para uma análise mais limpa, foram filtradas as tags que repetiam os Gêneros Principais (Ação, Aventura, etc.). Foram mantidas apenas tags descritivas de conteúdo ou estilo (ex: *Puzzle, VR, Story Rich*).

* *Observação:* apenas cerca de 23% dos jogos possuem essas tags descritivas (atribuídas por usuários).

---

## 📊 Fonte de Dados

Os dados utilizados são do dataset **Steam Store Games**, disponibilizado pelo usuário Nik Davis no Kaggle.

* **Abrangência:** mais de 27.000 jogos.
* **Período:** jogos lançados até o ano de 2020.
* **Dados Inclusos:** gênero, tempo médio de jogo, tags, avaliações, preço, desenvolvedora, entre outros.

![Preview da Tabela de Dados](img/fonte_steam_1.png)
*(Exemplo da estrutura dos dados brutos)*

🔗 **Links Úteis:**

* [Dataset no Kaggle](https://www.kaggle.com/nikdavis/steam-store-games)
* [Loja Steam](https://store.steampowered.com/?l=portuguese)
* [Documentação da API Steam](https://steamcommunity.com/dev?l=portuguese)

---

## 🛠 Tecnologias Utilizadas

* **Microsoft Power BI:** importação, transformação de dados (Power Query), modelagem e visualização.
* **DAX (Data Analysis Expressions):** criação das medidas de engajamento e popularidade.

---

## ⚠️ Disclaimer

Este é um **projeto acadêmico sem fins lucrativos**, realizado com base em dados públicos para fins de estudo. A Steam e a Valve Corporation não estão associadas à produção desta análise.

---

Desenvolvido por **Patrick Regis** — [LinkedIn](https://www.linkedin.com/in/patrickrgsanjos/)