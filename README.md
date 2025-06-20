# Classificação de Sementes de Trigo

Este projeto utiliza algoritmos de aprendizado de máquina para classificar tipos de sementes de trigo com base em características morfológicas medidas em laboratório.

## 📁 Estrutura do Projeto

O notebook `Graos.ipynb` contém todo o fluxo de trabalho:

1. **Leitura e pré-processamento dos dados**
   - Leitura de arquivo `.txt` contendo os dados brutos.
   - Conversão dos dados em um DataFrame do Pandas.
   - Tratamento de valores ausentes.
   - Renomeação de colunas com nomes descritivos.

2. **Análise exploratória**
   - Histogramas e boxplots por característica.
   - Gráficos de dispersão com separação por classe.
   - Verificação de valores ausentes.
   - Normalização e padronização das variáveis.

3. **Modelagem**
   - Divisão dos dados em treino (70%) e teste (30%).
   - Treinamento de 5 modelos: KNN, SVM, Random Forest, Naive Bayes e Regressão Logística.
   - Avaliação com métricas: acurácia, precisão, recall e F1-score.
   - Exibição de matrizes de confusão.

4. **Conclusão**
   - Random Forest apresentou o melhor desempenho.
   - Todos os modelos foram comparados em termos quantitativos.

## 📦 Requisitos

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter (opcional)

Instale as dependências com:

```bash
pip install -r requirements.txt
```

## 🚀 Execução

Abra o notebook com:

```bash
jupyter notebook Graos.ipynb
```

Ou execute passo a passo em outro ambiente Python.

## 📊 Resultados

O modelo Random Forest obteve acurácia acima de 90%, sendo o mais recomendado para esse problema. A classe 1 foi a mais difícil de classificar para todos os modelos, o que pode indicar sobreposição de características.
