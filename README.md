# Projecto_19
 
Análise de Pagamentos Inadimplentes Utilizando Modelos de Machine Learning

Com base no conjunto de dados disponível no UCI Machine Learning Repository, foram analisadas informações sobre pagamentos inadimplentes de clientes de cartão de crédito de Taiwan, abrangendo fatores como dados demográficos, histórico de crédito, pagamentos e extratos no período de abril a setembro de 2005.

O objetivo principal foi desenvolver e avaliar modelos preditivos para identificar clientes inadimplentes, auxiliando na tomada de decisão e na mitigação de riscos financeiros.

Tarefas Realizadas
Análise e Visualização Exploratória dos Dados (EDA):

Identificação de padrões nos dados, como taxas de inadimplência por faixa etária, limite de crédito e histórico de pagamentos.
Criação de visualizações (gráficos de dispersão, histogramas, heatmaps de correlação) para compreender a relação entre variáveis.
Preparação dos Dados:

Limpeza e tratamento de valores ausentes.
Normalização e codificação de variáveis categóricas.
Divisão do conjunto de dados em 70% para treinamento e 30% para teste.
Treinamento e Avaliação de Modelos Preditivos:

Treinamento e avaliação de seis classificadores de machine learning:
XGBoost
Support Vector Machine (SVM)
Naive Bayes
Regressão Logística
Random Forest
K-Nearest Neighbors (KNN)
Métricas utilizadas:
Acurácia
Precisão
Recall
F1-Score
Curva ROC e AUC (Área Sob a Curva)
Elaboração da Curva ROC:

Geração de curvas ROC para todos os modelos.
Comparação visual e quantitativa do desempenho dos classificadores em termos de AUC.


Resultados e Conclusões
Desempenho dos Modelos:

O Logistic Regression e o Random Forest destacaram-se como os melhores modelos:
Acurácia de 82% e F1-Score de 0.49 para a classe de inadimplentes.
Recall de 40% para identificar inadimplentes, o que é crucial no contexto do problema.
Modelos como Naive Bayes, apesar do recall alto (97%), apresentaram muitos falsos positivos, comprometendo a precisão geral.
XGBoost mostrou bom desempenho geral, mas um recall ligeiramente inferior aos melhores modelos.
Curva ROC e AUC:

Os modelos Random Forest e Logistic Regression apresentaram as melhores AUCs, demonstrando equilíbrio entre precisão e recall.
Conclusão Geral:

O problema de detecção de inadimplência apresenta desafios devido ao desequilíbrio de classes (inadimplentes são minoria).
Modelos como Random Forest e Logistic Regression proporcionam o melhor equilíbrio entre simplicidade, desempenho e capacidade de generalização.
Recomenda-se explorar técnicas adicionais, como reestruturação do conjunto de dados (SMOTE) ou ajustes de threshold, para melhorar ainda mais o recall da classe de inadimplentes.

Reflexão
Este projeto demonstra como diferentes algoritmos podem ser aplicados para resolver problemas práticos de classificação. Cada etapa, desde a análise exploratória até a avaliação de métricas, é essencial para garantir resultados confiáveis e alinhados com o objetivo do negócio.


Organização do Repositório notebooks/: Contém o notebook principal com a análise de dados, implementação dos modelos e relatórios de desempenho. data/: Arquivo de dados em formato CSV para fácil acesso e replicação do projeto.



