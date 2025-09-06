# 📊 Dashboard Financeiro – Power BI

Este projeto consiste em um **Dashboard Financeiro no Power BI**, desenvolvido para analisar **receitas, despesas e margem de lucro** de forma clara e dinâmica.  

O objetivo é oferecer uma visão gerencial que auxilie na **tomada de decisões estratégicas**, permitindo identificar os principais componentes que influenciam o desempenho financeiro.

---

## ⚙️ Recursos e KPIs

O dashboard inclui os seguintes indicadores principais:

- 📌 **Cartões de KPIs**
  - Total de Receitas
  - Total de Despesas
  - % Margem de Lucro

- 📊 **Gráfico de Barras Horizontais**
  - Distribuição do **total de receitas por componente** (aluguel, vendas, publicidade, etc.)

- 📉 **Gráfico em Área**
  - Evolução das **despesas por componente**

- 🧮 **Matriz**
  - Linhas: Tipo (**Receita/Despesa**) + Componentes  
  - Colunas: Anos  
  - Valores: totais calculados

- 🌟 **Principais Influenciadores**
  - Segmentos que mais impactam a variação de **Receita** e **Despesa**, analisados por tipo e componente.

---

## 🧾 Medidas criadas em DAX

Para cálculo dos KPIs, foram desenvolvidas medidas em **DAX**:

```DAX
TotalReceitas = SUM(Dados[Receita])
TotalDespesas = SUM(Dados[Despesa])
Lucro = [TotalReceitas] - [TotalDespesas]
MargemLucro = DIVIDE([Lucro], [TotalReceitas], 0)
````

Essas medidas foram utilizadas para compor tanto os cartões quanto as análises em gráficos e matrizes.

---

## 🖼️ Print do Dashboard

### 📌 Visão Geral
<img width="1387" height="765" alt="image" src="https://github.com/user-attachments/assets/bc7f22ba-b94c-45a2-904d-a068fa3498f1" />

---

## 🚀 Tecnologias utilizadas

* **Power BI Desktop**
* **Linguagem DAX** para criação de medidas
* **Modelagem de dados** e visualização interativa


