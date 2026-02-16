# 🍷 Classificação da Qualidade do Vinho com Random Forest

Projeto de **classificação multiclasse** usando **Random Forest** para prever a variável **`quality`** a partir de atributos físico químicos de vinhos. O notebook inclui **EDA**, preparação dos dados, treino, avaliação e **tuning com GridSearchCV** (métrica `f1_macro`).

## 🎯 Objetivo
Prever a qualidade do vinho (`quality`) e entender quais variáveis mais influenciam a classificação.

## 📦 Arquivos do repositório
- `README.md` guia do projeto
- `vinhos_random_forest_M32.ipynb` notebook com a análise e modelagem
- `winequality-red.csv` dataset usado no projeto

## 🧩 Dados
O dataset contém variáveis como acidez, açúcar residual, cloretos, SO2, densidade, pH, sulfatos e álcool.

**Target**
- `quality` (classes inteiras)

## 🔬 Metodologia
1. Carregamento do CSV e inspeção dos dados
2. Análise exploratória (distribuições, outliers, correlação)
3. Separação treino/teste
4. Random Forest baseline
5. Avaliação (acurácia, relatório de classificação, matriz de confusão)
6. Comparação de subconjuntos de features
7. Tuning com GridSearchCV (`f1_macro`)

## 📊 Resultados
O desempenho pode variar conforme o split e os hiperparâmetros. Em geral, o modelo tende a performar melhor nas classes mais frequentes e pior nas classes raras por conta do desbalanceamento.

## ▶️ Como executar
### 1. Instalar dependências
```bash
pip install pandas numpy scikit-learn matplotlib seaborn plotly jupyter
