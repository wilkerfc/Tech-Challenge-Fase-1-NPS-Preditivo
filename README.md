# 📊 Tech Challenge Fase 1 — NPS Preditivo

## Descrição do Projeto

Este repositório contém a solução completa do **Tech Challenge Fase 1** do curso de Data Science, com foco em **NPS Preditivo para E-commerce**. O objetivo é transformar dados operacionais em insights acionáveis e construir um modelo de Machine Learning capaz de prever se um cliente será um detrator antes da pesquisa de NPS ser aplicada.

---

## 📁 Estrutura do Repositório

```
nps_preditivo/
│
├── desafio_nps_fase_1.csv          # Dataset original (2.500 registros)
├── notebook_nps_preditivo.ipynb    # Notebook principal com toda a análise
├── requirements.txt                # Dependências do projeto
└── README.md                       # Este arquivo
```

---

## 🎯 Objetivos do Desafio

1. **Entendimento do Negócio** — Reflexão analítica sobre o problema de NPS em e-commerce
2. **Definição da Target** — Identificação e justificativa da variável alvo
3. **Análise Exploratória (EDA)** — Insights com foco em negócio
4. **Modelagem Preditiva** — Proposta e implementação de modelo de ML em Python

---

## 🔑 Principais Descobertas

| Fator | Impacto no NPS |
|---|---|
| `delivery_delay_days` | Correlação de **-0.60** com NPS (maior fator negativo) |
| `complaints_count` | Correlação de **-0.50** |
| `customer_service_contacts` | Correlação de **-0.35** |
| `repeat_purchase_30d` | Correlação de **+0.57** |
| `csat_internal_score` | Correlação de **+0.56** |

> ⚠️ **Ponto de ruptura crítico**: atrasos acima de 3 dias elevam a taxa de detratores para **93%**

---

## 🤖 Modelo Preditivo

- **Algoritmo**: Random Forest Classifier
- **Tarefa**: Classificação binária (Detrator vs Não-Detrator)
- **AUC-ROC**: **0.856**
- **Acurácia**: **84%**
- **Top Features**: `complaints_count`, `delivery_delay_days`, `order_value`

---

## 🚀 Como Executar

```bash
# 1. Clone o repositório
git clone https://github.com/seu-usuario/nps-preditivo.git
cd nps-preditivo

# 2. Instale as dependências
pip install -r requirements.txt

# 3. Abra o notebook
jupyter notebook notebook_nps_preditivo.ipynb
```

---

## 📦 Dependências

```
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
scikit-learn>=1.1.0
jupyter>=1.0.0
```

---

## 👥 Equipe

Desenvolvido como parte do **Tech Challenge — Pós-graduação em AI Scientist** - **wilkerfc**

---

## 📄 Licença

Este projeto é de uso acadêmico.
