# Análise e Previsão de Churn na Telecom X

## 📌 Objetivo do Projeto
Este projeto de Machine Learning tem como objetivo principal desenvolver um modelo preditivo para identificar clientes com alto risco de evasão (churn) na base de dados da empresa fictícia Telecom X. O foco é aplicar conceitos básicos de ciência de dados, desde o pré-processamento até a interpretação dos resultados, para gerar insights acionáveis.

## 🏗️ Estrutura do Projeto
O projeto foi desenvolvido seguindo uma metodologia de aprendizado supervisionado, dividida nas seguintes etapas:

1. **Pré-processamento**: Carregamento e limpeza dos dados, incluindo:
   - Remoção de colunas irrelevantes
   - Tratamento de valores ausentes
   - Codificação de variáveis categóricas

2. **Análise Exploratória**:
   - Investigação das características dos dados
   - Verificação do balanceamento de classes
   - Visualização de relações entre variáveis (boxplots e matriz de correlação)

3. **Modelagem**:
   - Divisão dos dados em conjuntos de treino e teste
   - Treinamento de dois modelos de classificação:
     - **Regressão Logística**: Modelo simples e interpretável (requer normalização)
     - **Random Forest**: Modelo robusto com alta performance (não sensível à escala)

4. **Avaliação e Interpretação**:
   - Análise de desempenho com métricas padrão
   - Identificação das variáveis mais importantes

5. **Conclusão e Recomendações**:
   - Resumo dos principais resultados
   - Proposição de estratégia para mitigar o churn

## 📊 Resultados e Métricas
Métricas de desempenho no conjunto de teste:

| Modelo               | Acurácia | Precisão | Recall | F1-Score |
|----------------------|----------|----------|--------|----------|
| Regressão Logística  | 0.8037   | 0.6558   | 0.5847 | 0.6183   |
| Random Forest        | 0.7963   | 0.6406   | 0.5977 | 0.6184   |

🔎 O modelo **Random Forest** demonstrou desempenho ligeiramente superior, especialmente em Recall e F1-Score, indicando melhor capacidade de identificar clientes que realmente cancelaram.

## 🔍 Principais Fatores de Evasão (Churn)
Os 3 fatores mais influentes na decisão de cancelamento:

1. **Tipo de Contrato**: Clientes com contratos mensais têm risco significativamente maior
2. **Tempo de Contrato**: Maior risco nos primeiros meses de serviço
3. **Total Gasto**: Clientes que gastaram menos têm mais probabilidade de cancelar

## 💡 Recomendação Estratégica
**Ação principal**: Fidelizar clientes de planos mensais e com pouco tempo de contrato, incentivando migração para planos anuais/longa duração através de:

- Ofertas exclusivas
- Promoções especiais
- Pacotes de benefícios

Esta estratégia visa reduzir a taxa de churn na origem, aumentando a retenção de clientes.
