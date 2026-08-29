# olist-data-analysis_FIAP
Análise de dados da Olist para avaliar a relação entre eficiência logística, satisfação e retenção de clientes no e-commerce.
# 📊 Olist — Logística, Satisfação e Retenção de Clientes

## 📌 Sobre o projeto

Este projeto apresenta uma análise de dados do **e-commerce brasileiro Olist**, com foco em investigar como o desempenho logístico pode estar relacionado à **satisfação e retenção de clientes**.

A análise utiliza dados de pedidos, entregas e avaliações dos clientes para identificar padrões relacionados ao cumprimento do prazo de entrega e à percepção de qualidade do serviço.

O projeto faz parte de um estudo de **Data Analysis / Data Science**, utilizando técnicas de tratamento, integração, exploração e visualização de dados.

---

## 🎯 Objetivo

Investigar a relação entre:

**Desempenho logístico → Satisfação do cliente → Retenção**

Entre os principais objetivos estão:

* Avaliar o cumprimento dos prazos de entrega;
* Identificar a proporção de pedidos atrasados;
* Analisar a distribuição das avaliações dos clientes;
* Comparar avaliações entre pedidos entregues no prazo e com atraso;
* Investigar possíveis relações entre atrasos e satisfação;
* Avaliar o comportamento de recompra dos clientes;
* Desenvolver indicadores que possam apoiar decisões relacionadas à logística e experiência do cliente.

---

## 🗂️ Dataset

O projeto utiliza o dataset público da **Olist**, contendo informações sobre pedidos realizados em uma plataforma brasileira de e-commerce.

Entre as principais bases utilizadas estão:

* `olist_orders_dataset.csv`
* `olist_order_reviews_dataset.csv`
* `olist_customers_dataset.csv`

As bases são relacionadas principalmente por meio dos identificadores de pedidos e clientes.

---

## 🔎 Principais análises

### 1. Perfil de entrega

Análise do cumprimento do prazo estimado de entrega.

Os pedidos são classificados como:

* **No prazo**
* **Com atraso**

A classificação é realizada comparando a data efetiva de entrega com a data estimada.

---

### 2. Distribuição das avaliações

As avaliações dos clientes são analisadas em uma escala de:

⭐ 1 a ⭐⭐⭐⭐⭐ 5 estrelas.

As avaliações também são agrupadas em três categorias:

| Grupo      | Classificação |
| ---------- | ------------- |
| ⭐⭐⭐⭐–⭐⭐⭐⭐⭐ | Positiva      |
| ⭐⭐⭐        | Intermediária |
| ⭐–⭐⭐       | Negativa      |

---

### 3. Atraso × Nota do cliente

Uma das análises do projeto compara a distribuição das avaliações entre:

**Pedidos entregues no prazo**

versus

**Pedidos entregues com atraso**

O objetivo é identificar se pedidos atrasados apresentam maior concentração de avaliações negativas.

### Exemplo da visualização

O gráfico utiliza:

* 🔵 Azul-claro para avaliações de 4–5 estrelas;
* 🟠 Laranja para avaliações de 3 estrelas;
* 🔴 Vermelho para avaliações de 1–2 estrelas.

As estrelas possuem contorno preto para melhorar a legibilidade.

---

## 🧮 Metodologia

O processo de análise segue as seguintes etapas:

```text
Carregamento dos dados
        ↓
Tratamento e validação
        ↓
Conversão das datas
        ↓
Remoção de registros incompletos
        ↓
Classificação das entregas
        ↓
Integração das bases
        ↓
Tratamento das avaliações
        ↓
Criação dos indicadores
        ↓
Análise exploratória
        ↓
Visualização dos resultados
        ↓
Interpretação
```

---

## 🛠️ Tecnologias

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Google Colab**
* **Jupyter Notebook**
* **GitHub**

---

## 📊 Principais resultados

Na análise de cumprimento do prazo, foram identificados:

* **91,89%** dos pedidos entregues no prazo;
* **8,11%** dos pedidos entregues com atraso.

Na distribuição geral das avaliações:

* ⭐⭐⭐⭐⭐ 5 estrelas: **57,78%**
* ⭐⭐⭐⭐ 4 estrelas: **19,29%**
* ⭐⭐⭐ 3 estrelas: **8,24%**
* ⭐⭐ 2 estrelas: **3,18%**
* ⭐ 1 estrela: **11,51%**

A análise de **atraso × nota** indica uma diferença relevante na distribuição das avaliações entre pedidos entregues no prazo e pedidos entregues com atraso.

Pedidos entregues no prazo apresentam maior concentração de avaliações positivas, enquanto os pedidos atrasados apresentam maior participação de avaliações negativas.

Esses resultados sugerem uma possível associação entre **desempenho logístico e satisfação do cliente**.

> **Importante:** a análise identifica associação entre as variáveis, mas não permite afirmar que o atraso seja, isoladamente, a causa da avaliação negativa. Outros fatores da experiência de compra também podem influenciar a satisfação.

---

## 📈 Próximas etapas

O projeto pode ser expandido com:

* Análise do tempo médio de entrega;
* Distribuição dos dias de atraso;
* Análise geográfica dos pedidos;
* Relação entre atraso e satisfação;
* Análise de recompra;
* Identificação de clientes recorrentes;
* Modelo preditivo de satisfação;
* Modelo de previsão de recompra;
* Simulação de diferentes níveis de SLA;
* Recomendações para melhoria da eficiência logística.

---

## 📁 Estrutura do projeto

```text
olist-data-analysis/
│
├── README.md
│
├── data/
│
├── notebooks/
│   ├── 01_exploracao.ipynb
│   ├── 02_perfil_entrega.ipynb
│   ├── 03_atrasos.ipynb
│   ├── 04_satisfacao.ipynb
│   └── 05_retencao.ipynb
│
├── outputs/
│   ├── graficos/
│   └── tabelas/
│
└── requirements.txt
```

---

## ⚠️ Dados

Os arquivos originais do dataset da Olist podem não ser incluídos diretamente neste repositório devido ao tamanho dos arquivos e às boas práticas de organização de projetos de dados.

O código foi desenvolvido para trabalhar com os arquivos CSV originais da base Olist.

---

## 👨‍💻 Autor

**Leonardo Abreu**

Projeto desenvolvido para análise de dados aplicada ao e-commerce, com foco em logística, satisfação e retenção de clientes.
