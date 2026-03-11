# 💰 Orçamento Familiar — Belo Horizonte, MG

<div align="center">

![Status](https://img.shields.io/badge/status-ativo-10b981?style=for-the-badge)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Dashboard financeiro interativo para gestão do orçamento familiar em Belo Horizonte**  
Casal + 1 filho · Renda R$ 11.000/mês · Metodologia 50·30·20

</div>

---

## 📋 Sobre o Projeto

Dashboard desenvolvido para acompanhamento e análise do orçamento familiar de um casal com 1 filho residente em bairro periférico de Belo Horizonte — MG.

O projeto nasceu da necessidade de visualizar de forma clara e interativa as finanças do mês, com projeções anuais, KPIs e análise de aderência ao modelo 50·30·20. É um arquivo HTML **standalone** — roda diretamente no navegador, sem backend, sem instalação.

---

## 🎯 Objetivos

- Monitorar despesas fixas, variáveis, cursos e investimentos mensais
- Avaliar a saúde financeira familiar com KPIs baseados no **Método dos 5 Passos**
- Aplicar e mensurar a aderência ao **modelo 50·30·20**
- Projetar o orçamento ao longo de 2026 com sazonalidade (IPTU, férias, Natal)
- Analisar os gastos com o filho separadamente
- Simular cenários **Orçado vs Realizado** por período

---

## 🗂️ Estrutura do Projeto

```
Orcamento_Familiar/
│
├── dashboard_orcamento_familiar.html   # Web App — dashboard completo
└── README.md
```

---

## 🖥️ Funcionalidades

### 📊 Aba — Visão Geral
- 6 cartões KPI: Renda, Fixas, Variáveis, Cursos, Reserva+Invest., Saldo Livre
- Gráfico de rosca com distribuição percentual do orçamento
- Gráfico de barras agrupadas — Orçado vs Realizado por categoria
- Barras de progresso — aderência ao modelo 50·30·20
- Tabela resumo com status por categoria

### 💸 Aba — Despesas
- Sistema de filtros interativo por item (chips clicáveis)
- Busca por nome de despesa em tempo real
- Filtro por categoria: Fixas, Variáveis e Cursos
- Seleção e deseleção individual com recálculo automático dos totais
- Gráfico de composição dos itens filtrados
- Mini análise: maior gasto, menor gasto e média por item

### 👶 Aba — Filho
- Tabela de gastos mensais com o filho (10 itens detalhados)
- Gráfico de barras horizontais por categoria
- Indicador de percentual da renda familiar comprometida

### 📅 Aba — Projeção Anual
- Gráfico de linha: Renda vs Despesas vs Saldo ao longo de 12 meses
- Gráfico de barras: Reserva de emergência acumulada vs meta de R$ 20.000
- Resumo consolidado do período selecionado

### 📈 Aba — KPIs
- 3 medidores visuais (gauges): Taxa de Sobra, Comprometimento Fixos e Comprometimento Filho
- Gráfico de equilíbrio de contribuição do casal
- Tabela de KPIs com resultado atual, meta e status

---

## 🔁 Filtros Globais

| Filtro | Opções |
|---|---|
| **Período** | Mar 2026 · T1 Jan–Mar · 1º Sem · Anual 2026 |
| **Cenário** | Orçado · Realizado (com multiplicadores sazonais) |

---

## 📐 Dados e Metodologia

### Composição do Orçamento Mensal Base

| Grupo | Total | % Renda |
|---|---|---|
| Despesas Fixas | R$ 3.060 | 27,8% |
| Despesas Variáveis | R$ 2.700 | 24,5% |
| Cursos | R$ 400 | 3,6% |
| Reserva + Investimento | R$ 880 | 8,0% |
| **Saldo Livre** | **R$ 3.960** | **36,0%** |
| **Renda Total** | **R$ 11.000** | 100% |

### Sazonalidade
Multiplicadores mensais aplicados no cenário **Realizado** para simular variações reais do custo de vida em BH:

| Jan | Fev | Mar | Abr | Mai | Jun | Jul | Ago | Set | Out | Nov | Dez |
|---|---|---|---|---|---|---|---|---|---|---|---|
| +12% | -3% | 0% | -5% | -3% | +1% | +8% | -4% | -6% | -2% | +2% | +18% |

> Jan: IPTU · Jul: férias escolares · Dez: Natal e presentes

### KPIs Monitorados

| KPI | Meta | Resultado | Status |
|---|---|---|---|
| Taxa de Sobra | ≥ 15% | 36,0% | ✅ |
| Comprometimento Fixos | ≤ 50% | 27,8% | ✅ |
| Comprometimento Filho | ≤ 20% | 7,9% | ✅ |
| Investimento | ≥ 5% | 3,0% | ⚠️ |
| Equilíbrio do Casal | Δ ≤ 5% | 0,0% | ✅ |

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Versão | Uso |
|---|---|---|
| **HTML5** | — | Estrutura do dashboard |
| **CSS3** | — | Estilo, variáveis e animações |
| **JavaScript** | ES6+ | Lógica de cálculo, filtros e renderização |
| **Chart.js** | 4.4.0 | Gráficos (rosca, barras, linha, gauge) |
| **Google Fonts** | — | DM Sans + DM Mono |

---

## 🚀 Como Usar

```bash
# Clone o repositório
git clone https://github.com/Lucasmelg97/Orcamento_Familiar.git

# Abra o arquivo diretamente no navegador
# Não requer servidor, instalação ou dependências
open dashboard_orcamento_familiar.html
```

Ou simplesmente **baixe o arquivo HTML** e abra com qualquer navegador moderno.

---

## 🎨 Design System

| Token | Valor | Uso |
|---|---|---|
| `--bg` | `#0f1117` | Fundo da página |
| `--surface` | `#1a1d27` | Cards e painéis |
| `--border` | `#2d3148` | Bordas |
| `--accent` | `#4f8ef7` | Azul principal |
| `--orange` | `#f97316` | Despesas Fixas |
| `--warn` | `#f59e0b` | Variáveis |
| `--purple` | `#8b5cf6` | Cursos |
| `--cyan` | `#06b6d4` | Reserva |
| `--green` | `#10b981` | Saldo / Status OK |

---

## 👤 Autor

**Lucas Santiago Vieira Melgaço**  
Data Enginner · Belo Horizonte, MG

[![GitHub](https://img.shields.io/badge/GitHub-Lucasmelg97-181717?style=flat&logo=github)](https://github.com/Lucasmelg97)

---

## 📄 Licença

Este projeto é de uso pessoal e educacional.  
Sinta-se à vontade para adaptar para o seu próprio orçamento familiar.

---

<div align="center">
  <sub>Feito com 💙 em Belo Horizonte · Metodologia 50·30·20 + KPIs em 5 Passos</sub>
</div>
