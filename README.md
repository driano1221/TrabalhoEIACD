
# Assignment No. 2 - Data Exploration and Enrichment for Supervised Classification

## Descrição do Projeto
Este projeto tem como objetivo desenvolver um pipeline completo de ciência de dados para abordar um caso de uso real utilizando o conjunto de dados Hepatocellular Carcinoma (HCC). O objetivo principal é criar um modelo de aprendizado de máquina capaz de prever a sobrevivência dos pacientes 1 ano após o diagnóstico (classificando como "vive" ou "morre").

## Etapas do Projeto

1. **Exploração de Dados**
   - Análise exploratória inicial dos dados
   - Exame dos tipos de variáveis, número de registros, distribuição de classes, valores por atributo, inconsistências, etc.

2. **Pré-processamento de Dados**
   - Imputação de valores ausentes
   - Transformação de dados, escala, engenharia de variáveis (criação de novas variáveis ou remoção de variáveis redundantes)

3. **Modelagem de Dados (Aprendizado Supervisionado)**
   - Definição dos conjuntos de treinamento e teste
   - Seleção e parametrização de algoritmos de aprendizado
   - Avaliação do processo de aprendizado

4. **Avaliação de Dados**
   - Comparação dos resultados da classificação usando diferentes métricas de avaliação e visualizações

5. **Interpretação dos Resultados**
   - Extração de insights significativos dos resultados obtidos
   - Explicação do comportamento dos modelos
   - Recomendações para análises futuras

## Conjunto de Dados

**Descrição da Base de Dados HCC:**

A base de dados HCC é composta por 50 variáveis (colunas) e múltiplos registros de pacientes (linhas). Cada linha representa um paciente diagnosticado com carcinoma hepatocelular. As variáveis abrangem características demográficas, clínicas e laboratoriais dos pacientes.

### Variáveis da Base de Dados

1. Gender: Gênero do paciente (Male/Female)
2. Symptoms: Presença de sintomas (Yes/No)
3. Alcohol: Consumo de álcool (Yes/No)
4. HBsAg, HBeAg, HBcAb, HCVAb: Resultados de testes para hepatite B e C (Yes/No)
5. Cirrhosis: Presença de cirrose (Yes/No)
...
37. Creatinine: Nível de creatinina (mg/dL)
38. Nodules: Número de nódulos hepáticos
39. Major_Dim: Tamanho do maior nódulo (cm)
40. Dir_Bil: Bilirrubina direta (mg/dL)
41. Iron: Nível de ferro (ug/dL)
42. Sat: Saturação de transferrina (%)
43. Ferritin: Nível de ferritina (ng/mL)
44. **Class**: Classe de sobrevivência após 1 ano (Lives/Dies)

## Requisitos

Certifique-se de ter os seguintes pacotes instalados para executar o código do projeto:

```bash
pip install numpy pandas seaborn matplotlib scikit-learn
```

## Executando o Código



1. **Abra o Jupyter Notebook:**
   ```bash
   jupyter notebook TrabalhoCDIA.ipynb
   ```

2. **Execute as Células:**
   - Siga a ordem das células no notebook para executar cada etapa do pipeline de ciência de dados.

## Principais Bibliotecas Utilizadas

- **numpy:** Para operações matemáticas e manipulação de arrays.
- **pandas:** Para manipulação e análise de dados.
- **seaborn e matplotlib:** Para visualizações de dados.
- **scikit-learn:** Para modelagem e avaliação de aprendizado de máquina.

## Análise Exploratória de Dados

Realizamos a análise exploratória inicial dos dados, incluindo a visualização de distribuições de variáveis, detecção e tratamento de valores ausentes, e identificação de outliers.

## Pré-processamento de Dados

Realizamos o pré-processamento dos dados, incluindo imputação de valores ausentes, transformação e normalização de variáveis, e engenharia de variáveis.

## Modelagem e Avaliação

Utilizamos diversos algoritmos de aprendizado de máquina, incluindo Decision Tree, Random Forest, KNN, Logistic Regression, Gradient Boosting, XGBoost e MLP. Realizamos otimização de hiperparâmetros e avaliamos os modelos usando métricas como precisão, recall, F1-score e ROC AUC.

## Resultados e Interpretação

Os melhores modelos foram RandomForestClassifier, LogisticRegression e XGBClassifier. Estes modelos apresentaram um bom equilíbrio entre precisão, recall e F1-score, com um ROC AUC acima de 0.85. A análise das características mais importantes indicou que variáveis relacionadas à função hepática e ao estado geral do paciente são cruciais para a previsão de sobrevivência.

## Conclusão

Este projeto demonstra um pipeline completo de ciência de dados, desde a exploração e pré-processamento dos dados até a modelagem e avaliação de aprendizado de máquina, proporcionando insights significativos sobre os fatores que influenciam a sobrevivência de pacientes com carcinoma hepatocelular.


