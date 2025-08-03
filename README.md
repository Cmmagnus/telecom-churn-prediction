# 📡 Telecom X – Parte 2: Prevendo a Evasão de Clientes

<p align="center">
  <img src="assets/banner_readme.png" alt="Banner Telecom X" style="width:100%; max-width:800px;">
</p>

# 📉 Previsão de Evasão de Clientes – Projeto Telecom X (Parte 2)

Este projeto faz parte do desafio **Telecom X – Geração ONE/Alura**, com o objetivo de analisar dados de uma operadora de telecomunicações e **prever a evasão de clientes (churn)** utilizando técnicas de **Data Science e Machine Learning**.

---

## 🎯 Objetivo

Construir um modelo preditivo confiável que permita **identificar clientes com alto risco de evasão**, além de explorar os **fatores determinantes do churn**, contribuindo com **estratégias de retenção** mais eficazes.

---

## 🧠 Tecnologias Utilizadas

- `Python 3.10`
- `Pandas` e `NumPy`
- `Matplotlib` e `Seaborn`
- `Scikit-learn`
- `Google Colab / Jupyter Notebook`

---

## 📁 Estrutura do Repositório

```
TELECOM_X-BR-PART_2/
├── assets/                     # Gráficos gerados na análise
│   ├── distribuicao_churn.png
│   ├── boxplot_tenure_vs_churn.png
│   ├── matriz_correlacao.png
│   ├── scatter_total_vs_tenure_churn.png
│   ├── matriz_regressão_logística.png
│   ├── matriz_random_forest.png
│   ├── top15_coeficientes_regressao_logistica.png
│   └── top15_importancia_random_forest.png
│
├── data/                       # Bases tratadas para modelagem
│   ├── base_pronta_para_modelos.csv
│   └── df_normalizado_final.csv
│
├── documents/                  # Documentos auxiliares
│   └── Descricao.docx
│
├── notebook/                   # Scripts e relatórios
│   ├── estudo_de_dados.ipynb
│   └── Relatorio_Evasao_Telecom.md
```

---

## 📈 Principais Etapas do Projeto

### 🔍 Análise Exploratória (EDA)
- Verificação de **desequilíbrio nas classes**
- Análise da relação entre **tempo de contrato**, **gastos** e **churn**
- Estudo de **correlação entre variáveis**

### 🤖 Modelagem Preditiva
Modelos aplicados:
- **Regressão Logística** (com normalização)
- **Random Forest** (sem normalização)

> Ambos os modelos foram avaliados com acurácia, precisão, recall e F1-score.

---

## 📊 Resultados

| Modelo              | Acurácia | Precisão | Recall | F1-Score |
|---------------------|----------|----------|--------|----------|
| Regressão Logística | 98.0%    | 100%     | 92.5%  | 96.1%    |
| Random Forest       | 98.7%    | 100%     | 95.4%  | 97.6%    |

✅ O modelo de **Random Forest** obteve o melhor desempenho geral.

📌 **Impacto das variáveis no churn:**

![Impacto das variáveis no churn](./assets/top15_importancia_random_forest.png)

---

## 🔎 Fatores Mais Relevantes para o Churn

- Baixo tempo de contrato (`tenure`)
- Pagamento por boleto bancário
- Contratos mensais
- Adesão a múltiplos serviços opcionais
- Variáveis relacionadas ao suporte e atendimento

---

## 💡 Recomendações Estratégicas

1. **Incentivar contratos mais longos**, como anuais
2. **Bonificar o uso de débito automático**
3. Criar **pacotes personalizados** para clientes com muitos serviços
4. Atuar preventivamente com clientes **novos ou com sinais de evasão**
5. **Reforçar suporte técnico** e canais de atendimento

---

## 📄 Documentação

O relatório completo encontra-se em:
- [`notebook/Relatorio_Evasao_Telecom.md`](notebook/Relatorio_Evasao_Telecom.md)

---

## 👤 Autor

**Carlos M. Marcelino**  
 | Cientista de Dados em Formação |  
🔗 [LinkedIn](https://www.linkedin.com/in/carlos-magno-marcelino-619ab9186/) · 💻 [GitHub](https://github.com/Cmmagnus/)

---

## 🏁 Status

✅ Projeto Finalizado  
📦 Pronto para apresentação, versionamento e deploy em painéis (ex: Streamlit)

---

## 📜 Licença

Este projeto está sob a licença **MIT**. Sinta-se livre para utilizá-lo com os devidos créditos.
