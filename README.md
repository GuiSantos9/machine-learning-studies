Esta é a versão consolidada do núcleo de ML clássico. Os blocos ligados ao Scikit-Learn abrangem suas áreas de aprendizado supervisionado e não supervisionado, transformações, avaliação, inspeção e computação.

### Formulação do problema

- [ ] Diferenciar IA, Machine Learning e Deep Learning.

- [ ] Diferenciar aprendizado supervisionado, não supervisionado e por reforço.

- [ ] Diferenciar aprendizado semissupervisionado, autossupervisionado, ativo e online.

- [ ] Diferenciar regressão, classificação, agrupamento, ranking e detecção de anomalias.

- [ ] Identificar amostra, atributo, alvo, previsão e rótulo.

- [ ] Definir a unidade de observação: pessoa, transação, documento, dispositivo ou evento.

- [ ] Definir população-alvo, momento da previsão e horizonte do alvo.

- [ ] Verificar se os atributos estarão disponíveis no momento da inferência.

- [ ] Distinguir previsão, descrição, explicação e decisão.

- [ ] Traduzir o objetivo do problema em métrica e critério de sucesso.

- [ ] Identificar custos distintos de falsos positivos e falsos negativos.

- [ ]  Criar baselines simples, heurísticos e não baseados em ML.

- [ ]  Documentar quando não usar Machine Learning.

### Fundamentos do aprendizado

- [ ] Explicar treinamento, validação, teste e inferência.

- [ ] Diferenciar parâmetros aprendidos de hiperparâmetros.

- [ ] Reconhecer overfitting e underfitting.

- [ ] Explicar o trade-off viés–variância e suas limitações como diagnóstico.

- [ ] Relacionar capacidade do modelo, quantidade de dados e generalização.

- [ ] Diferenciar função de perda de métrica de avaliação.

- [ ] Explicar risco empírico e objetivo de generalização.

- [ ] Identificar viés indutivo em diferentes famílias de modelos.

- [ ] Diferenciar modelos paramétricos e não paramétricos.

- [ ] Diferenciar modelos discriminativos e generativos.

- [ ] Diferenciar interpolação e extrapolação.

- [ ] Explicar regularização explícita e controle de capacidade.

- [ ] Reconhecer situações em que a hipótese de dados independentes é inadequada.

- [ ] Distinguir ruído nos atributos, ruído nos rótulos e insuficiência de informação.

- [ ]  Investigar discrepâncias entre desempenho de treino e validação.

### Dados e qualidade dos rótulos

- [ ] Identificar atributos numéricos, categóricos, ordinais, temporais e textuais.

- [ ] Investigar distribuições, valores ausentes, valores extremos e inconsistências.

- [ ] Identificar duplicatas e quase duplicatas.

- [ ] Detectar entidades repetidas e dependência entre observações.

- [ ] Investigar cardinalidade, categorias raras e identificadores.

- [ ] Analisar distribuição do alvo e cobertura dos diferentes segmentos.

- [ ] Verificar consistência da definição e da coleta dos rótulos.

- [ ] Investigar erro de anotação, atraso do rótulo e exemplos ambíguos.

- [ ] Reconhecer vieses de seleção, sobrevivência e disponibilidade de rótulos.

- [ ] Investigar dados ausentes informativos e limites da imputação.

- [ ]  Construir um relatório de qualidade dos dados.

- [ ]  Versionar dados e registrar sua procedência.

### Particionamento e leakage

O conjunto de teste não deve orientar escolhas do modelo; pré-processamento e seleção de atributos também podem produzir vazamento quando ajustados antes da separação adequada.

- [ ] Separar treino, validação e teste com funções distintas.

- [ ] Usar divisão aleatória apenas quando compatível com o problema.

- [ ] Usar estratificação quando apropriado.

- [ ] Separar por pessoa, cliente, dispositivo, instituição ou outra entidade.

- [ ] Separar cronologicamente quando o uso real envolve previsão futura.

- [ ] Detectar atributos derivados direta ou indiretamente do alvo.

- [ ] Detectar informações produzidas depois do momento da previsão.

- [ ] Detectar leakage por duplicação e entidades compartilhadas.

- [ ] Ajustar imputadores, escaladores e seletores somente no treino.

- [ ] Refazer transformações aprendidas dentro de cada fold.

- [ ] Validar agregações e joins conforme a disponibilidade histórica dos dados.

- [ ]  Manter o teste final isolado das decisões iterativas.

- [ ]  Auditar o fluxo completo, não apenas a chamada de treinamento.

### API do Scikit-Learn

- [ ] Dominar fit, transform, fit_transform e predict.

- [ ] Diferenciar predict_proba, decision_function e score.

- [ ] Interpretar atributos aprendidos terminados em _.

- [ ] Dominar get_params, set_params e parâmetros com __.

- [ ] Entender clonagem de estimadores em validação e busca.

- [ ] Trabalhar com arrays, DataFrames e matrizes esparsas.

- [ ] Preservar nomes com get_feature_names_out e set_output.

- [ ] Controlar aleatoriedade com random_state.

- [ ] Interpretar avisos de convergência e incompatibilidade.

- [ ] Diferenciar warm_start de partial_fit.

- [ ] Entender passagem de sample_weight, grupos e outros metadados.

- [ ]  Consultar a documentação da versão efetivamente utilizada.

### Pré-processamento numérico

Os escaladores, normalizadores e transformações não lineares resolvem problemas diferentes; normalizar amostras não é o mesmo que padronizar colunas.

- [ ] Comparar StandardScaler, MinMaxScaler, RobustScaler e MaxAbsScaler.

- [ ] Distinguir escalonamento de atributos de normalização por amostra.

- [ ] Aplicar Normalizer quando a representação exigir norma unitária.

- [ ] Identificar modelos sensíveis à escala e modelos pouco sensíveis.

- [ ] Usar SimpleImputer com estratégias adequadas.

- [ ] Comparar imputação simples e KNNImputer.

- [ ] Conhecer imputação multivariada com IterativeImputer.

- [ ] Adicionar indicadores de ausência quando pertinente.

- [ ] Conhecer modelos que aceitam valores ausentes nativamente.

- [ ] Aplicar transformações logarítmicas respeitando o domínio.

- [ ] Comparar Box–Cox, Yeo–Johnson e transformação por quantis.

- [ ] Avaliar discretização com KBinsDiscretizer.

- [ ] Avaliar efeitos das transformações sobre distâncias e relações entre atributos.

- [ ]  Evitar densificação acidental de matrizes esparsas.

### Pré-processamento categórico

- [ ] Diferenciar categorias nominais e ordinais.

- [ ] Usar OneHotEncoder e compreender a expansão de dimensionalidade.

- [ ] Usar OrdinalEncoder sem introduzir ordenação indevida.

- [ ] Reservar LabelEncoder à codificação do alvo quando necessária.

- [ ] Tratar categorias desconhecidas na inferência.

- [ ] Agrupar categorias raras e limitar cardinalidade.

- [ ] Tratar ausência como categoria quando adequado.

- [ ] Comparar one-hot, frequência, hashing e target encoding.

- [ ] Entender suavização e cross-fitting no target encoding.

- [ ] Adaptar codificações supervisionadas ao protocolo temporal ou por grupos.

- [ ]  Testar categorias novas, ausentes e extremamente raras.

- [ ]  Comparar codificação externa com tratamento categórico nativo do modelo.

### Engenharia de atributos

- [ ] Criar interações, razões e diferenças justificadas pelo domínio.

- [ ] Construir atributos polinomiais sem expansão indiscriminada.

- [ ] Usar funções de base e splines.

- [ ] Extrair componentes de datas e durações.

- [ ] Representar variáveis cíclicas, como hora e mês.

- [ ] Construir contagens, frequências e agregações por entidade.

- [ ] Construir agregações históricas sem incorporar informação futura.

- [ ] Transformar o alvo com TransformedTargetRegressor.

- [ ] Avaliar consequências de inverter transformações do alvo.

- [ ]  Comparar atributos novos por ablação.

- [ ]  Documentar disponibilidade, custo e significado de cada atributo.

- [ ]  Remover atributos que não existem no ambiente real de previsão.

### Seleção de atributos

O Scikit-Learn diferencia métodos de filtragem, seleção baseada em modelos e procedimentos iterativos; essa etapa deve integrar a validação, e não antecedê-la usando todo o dataset.

- [ ] Diferenciar seleção de atributos de extração de componentes.

- [ ] Remover atributos constantes com VarianceThreshold.

- [ ] Conhecer filtros univariados com SelectKBest e SelectPercentile.

- [ ] Comparar associação linear e informação mútua.

- [ ] Reconhecer limitações da seleção baseada apenas em correlação.

- [ ] Usar SelectFromModel.

- [ ] Usar RFE e RFECV.

- [ ] Conhecer seleção sequencial de atributos.

- [ ] Avaliar redundância e estabilidade da seleção entre folds.

- [ ]  Comparar desempenho, custo e simplicidade antes e depois da seleção.

### Pipelines e composição

- [ ] Construir Pipeline e make_pipeline.

- [ ] Usar ColumnTransformer e make_column_transformer.

- [ ] Combinar representações com FeatureUnion.

- [ ] Buscar hiperparâmetros do pré-processamento e do modelo conjuntamente.

- [ ] Usar FunctionTransformer para transformações apropriadas.

- [ ] Implementar transformadores com BaseEstimator e TransformerMixin.

- [ ] Preservar nomes, formatos e consistência das saídas.

- [ ]  Testar compatibilidade com clonagem e validação cruzada.

- [ ]  Usar cache quando útil e controlar consumo de memória.

- [ ]  Persistir o fluxo de transformação junto do estimador.

### Regressão linear e extensões

- [ ] Implementar regressão linear simples e múltipla.

- [ ] Interpretar intercepto, coeficientes e escala dos atributos.

- [ ] Analisar resíduos e falhas sistemáticas.

- [ ] Investigar multicolinearidade e instabilidade dos coeficientes.

- [ ] Comparar Ridge, Lasso e Elastic Net.

- [ ] Entender o efeito de alpha e l1_ratio.

- [ ] Usar regressão polinomial e splines como extensões da representação.

- [ ] Implementar regressão com SGD.

- [ ] Comparar Huber, RANSAC e Theil–Sen.

- [ ] Implementar regressão quantílica.

- [ ] Conhecer regressões Poisson, Gamma e Tweedie.

- [ ] Conhecer BayesianRidge e ARDRegression.

- [ ] Conhecer LARS e Orthogonal Matching Pursuit como aprofundamento.

- [ ]  Escolher modelos considerando o alvo, o erro, a estabilidade e a validação — não apenas multicolinearidade.

### Classificação linear e discriminante

- [ ] Implementar regressão logística binária.

- [ ] Diferenciar logit, probabilidade e limiar de decisão.

- [ ] Interpretar coeficientes sem confundir associação com causalidade.

- [ ] Comparar regularização L1, L2 e Elastic Net.

- [ ] Entender a relação entre C e força da regularização.

- [ ] Implementar classificação multinomial.

- [ ] Conhecer SGDClassifier, perceptron e métodos passivo-agressivos.

- [ ] Comparar Linear Discriminant Analysis e Quadratic Discriminant Analysis.

- [ ] Identificar hipóteses distribucionais de LDA e QDA.

- [ ] Avaliar shrinkage em estimação de covariância.

- [ ]  Comparar fronteira de decisão, discriminação e calibração.

### Vizinhos, Naive Bayes e kernels

- [ ] Implementar KNN para classificação e regressão.

- [ ] Comparar ponderação uniforme e por distância.

- [ ] Analisar n_neighbors, métricas de distância e escala.

- [ ] Avaliar custo de busca e degradação em alta dimensionalidade.

- [ ] Diferenciar Gaussian, Multinomial, Bernoulli, Complement e Categorical Naive Bayes.

- [ ] Explicar independência condicional e suavização.

- [ ]  Aplicar Naive Bayes respeitando a representação dos dados.

- [ ] Implementar SVC, LinearSVC e SVR.

- [ ] Explicar margem, vetores de suporte e efeito de C.

- [ ] Comparar kernels linear, polinomial e RBF.

- [ ] Analisar gamma, epsilon e sensibilidade à escala.

- [ ] Conhecer Kernel Ridge.

- [ ] Conhecer aproximações de kernels com Nyström e random features.

- [ ]  Comparar desempenho e escalabilidade de métodos lineares e kernelizados.

### Árvores e ensembles

- [ ] Implementar árvores para classificação e regressão.

- [ ] Diferenciar critérios de classificação e de regressão.

- [ ] Interpretar Gini, entropia e redução de impureza.

- [ ] Ajustar profundidade, tamanho mínimo de folhas e divisão de nós.

- [ ] Aplicar poda por complexidade com ccp_alpha.

- [ ] Explicar bootstrap e bagging.

- [ ] Implementar Random Forest e Extra Trees.

- [ ] Interpretar avaliação out-of-bag e suas condições de uso.

- [ ] Analisar diversidade e correlação entre os componentes do ensemble.

- [ ] Implementar AdaBoost e Gradient Boosting.

- [ ] Relacionar boosting à otimização de uma função de perda.

- [ ] Ajustar learning rate, número de árvores e complexidade das árvores.

- [ ] Implementar HistGradientBoostingClassifier e HistGradientBoostingRegressor.

- [ ] Conhecer restrições monotônicas e de interação quando disponíveis.

- [ ] Implementar voting com votos e probabilidades.

- [ ] Implementar stacking usando previsões out-of-fold.

- [ ]  Avaliar early stopping sem contaminar a avaliação final.

- [ ]  Comparar ensembles com modelos mais simples sob o mesmo orçamento.

### Boosting externo

- [ ] Implementar XGBoost, LightGBM e CatBoost.

- [ ] Identificar diferenças nas APIs, parâmetros e formatos de entrada.

- [ ] Comparar políticas de crescimento das árvores.

- [ ] Entender treinamento por histogramas.

- [ ] Estudar tratamento de categorias e valores ausentes em cada biblioteca.

- [ ] Estudar regularização e amostragem de linhas e atributos.

- [ ] Estudar ordered boosting e codificações ordenadas no CatBoost.

- [ ]  Configurar objetivos, métricas e early stopping corretamente.

- [ ]  Avaliar CPU, GPU, memória e latência no problema concreto.

- [ ]  Evitar atribuir superioridade universal a uma biblioteca.

### Outros modelos supervisionados

O guia do Scikit-Learn também inclui problemas multiclass, multilabel e multioutput, além de redes MLP; essas competências não devem ficar implícitas em “classificação”.

- [ ] Diferenciar classificação binária, multiclass e multilabel.

- [ ] Diferenciar regressão de saída única e multioutput.

- [ ] Comparar estratégias one-vs-rest e one-vs-one.

- [ ] Conhecer classifier chains e regressor chains.

- [ ] Implementar regressão isotônica.

- [ ] Conhecer Gaussian Process Regression e Classification.

- [ ] Interpretar kernels e incerteza preditiva em processos gaussianos.

- [ ] Conhecer MLPClassifier e MLPRegressor como ponte para redes neurais.

- [ ]  Avaliar se a formulação de saída corresponde ao problema real.

### Clusterização

- [ ] Formular o objetivo do agrupamento sem depender apenas de um gráfico.

- [ ] Implementar K-Means e K-Means++.

- [ ] Analisar inicialização, número de clusters e diferentes execuções.

- [ ] Implementar MiniBatchKMeans.

- [ ] Comparar distâncias e efeitos do pré-processamento.

- [ ] Implementar agrupamento hierárquico aglomerativo.

- [ ] Comparar single, complete, average e Ward linkage.

- [ ] Interpretar dendrogramas.

- [ ] Implementar DBSCAN e analisar eps e min_samples.

- [ ] Conhecer OPTICS e HDBSCAN.

- [ ] Conhecer clustering espectral.

- [ ] Conhecer Mean Shift, Affinity Propagation e BIRCH.

- [ ] Comparar Gaussian Mixture Models com agrupamentos rígidos.

- [ ]  Avaliar estabilidade, utilidade e perfis dos grupos.

- [ ]  Definir como atribuir novos exemplos ou atualizar os agrupamentos.

### Redução de dimensionalidade

- [ ] Implementar PCA e interpretar variância explicada.

- [ ] Diferenciar componentes principais de atributos originais.

- [ ] Avaliar padronização, número de componentes e reconstrução.

- [ ] Conhecer whitening e suas consequências.

- [ ] Implementar IncrementalPCA e TruncatedSVD.

- [ ] Conhecer Kernel PCA e Sparse PCA.

- [ ] Conhecer NMF e restrições de não negatividade.

- [ ] Diferenciar PCA, análise fatorial e ICA.

- [ ] Conhecer dictionary learning e projeções aleatórias.

- [ ] Usar t-SNE e UMAP para exploração.

- [ ] Analisar sensibilidade a hiperparâmetros e sementes.

- [ ] Evitar tratar agrupamentos visuais como confirmação automática de estrutura.

- [ ]  Avaliar a representação pela tarefa subsequente, não apenas pelo gráfico.

### Anomalias e estimação de densidade

- [ ] Diferenciar outlier, novidade, erro de dados e evento raro.

- [ ] Diferenciar detecção supervisionada e não supervisionada de anomalias.

- [ ] Implementar Isolation Forest.

- [ ] Implementar Local Outlier Factor.

- [ ] Diferenciar uso do LOF para outliers e para novidade.

- [ ] Implementar One-Class SVM.

- [ ] Conhecer Elliptic Envelope e covariância robusta.

- [ ] Entender score de anomalia e limiar de decisão.

- [ ] Estudar Kernel Density Estimation e seleção de bandwidth.

- [ ] Conhecer misturas gaussianas para densidade.

- [ ]  Avaliar alertas com dados rotulados quando disponíveis.

- [ ]  Considerar capacidade de investigação e custo dos falsos alarmes.

### Avaliação de regressão

- [ ] Calcular MAE, MSE e RMSE.

- [ ] Interpretar sensibilidade a erros extremos.

- [ ] Interpretar R², inclusive valores negativos.

- [ ] Conhecer erro absoluto mediano.

- [ ] Avaliar MAPE com atenção a alvos nulos ou próximos de zero.

- [ ] Definir explicitamente WAPE/WMAPE e a convenção usada.

- [ ] Avaliar métricas em escala original e transformada.

- [ ] Conhecer pinball loss para quantis.

- [ ] Conhecer deviance para objetivos Poisson, Gamma e Tweedie.

- [ ]  Comparar com DummyRegressor.

- [ ]  Analisar resíduos por faixa do alvo, segmento e tempo.

### Avaliação de classificação

- [ ] Interpretar matriz de confusão.

- [ ] Calcular acurácia, precisão, recall e F1.

- [ ] Conhecer especificidade, balanced accuracy e F-beta.

- [ ] Comparar médias macro, micro, weighted e resultados por classe.

- [ ] Conhecer Matthews correlation coefficient e Cohen’s kappa.

- [ ] Interpretar ROC e ROC-AUC.

- [ ] Interpretar curva precision–recall.

- [ ] Diferenciar average precision de integração trapezoidal da curva PR.

- [ ] Investigar influência da prevalência na interpretação dos resultados.

- [ ] Calcular log loss e Brier score.

- [ ] Conhecer top-k accuracy quando apropriada.

- [ ] Avaliar multilabel com métricas apropriadas.

- [ ]  Comparar com DummyClassifier.

- [ ]  Reportar métricas por classe e por segmentos relevantes.

### Avaliação não supervisionada

- [ ] Calcular silhouette, Davies–Bouldin e Calinski–Harabasz.

- [ ] Interpretar limitações dessas métricas para diferentes geometrias.

- [ ] Usar ARI, AMI ou outras métricas externas quando existir referência.

- [ ] Avaliar estabilidade dos agrupamentos entre amostras e sementes.

- [ ] Avaliar reconstrução em decomposições quando pertinente.

- [ ]  Validar utilidade dos resultados no domínio.

- [ ]  Não escolher automaticamente a solução com melhor métrica interna.

### Validação e seleção de modelos

- [ ] Usar KFold e StratifiedKFold.

- [ ] Usar GroupKFold e divisões por grupo.

- [ ] Usar StratifiedGroupKFold quando compatível com o problema.

- [ ] Usar TimeSeriesSplit e avaliar suas limitações.

- [ ] Construir validação temporal com gaps ou bloqueios quando necessário.

- [ ] Usar cross_validate com múltiplas métricas.

- [ ] Produzir previsões out-of-fold com cross_val_predict.

- [ ] Diferenciar previsões out-of-fold de estimativa final de desempenho.

- [ ] Implementar nested cross-validation.

- [ ] Interpretar variabilidade entre folds.

- [ ] Construir curvas de aprendizado e validação.

- [ ] Conhecer testes por permutação de desempenho.

- [ ]  Comparar modelos nas mesmas divisões.

- [ ]  Evitar escolher modelos a partir de diferenças pequenas e instáveis.

### Otimização de hiperparâmetros

- [ ] Implementar GridSearchCV e RandomizedSearchCV.

- [ ] Definir espaços coerentes com o comportamento dos parâmetros.

- [ ] Usar escalas logarítmicas quando adequadas.

- [ ] Definir espaços condicionais.

- [ ] Conhecer successive halving.

- [ ] Usar otimização baseada em modelos com Optuna ou alternativa equivalente.

- [ ] Entender pruning e interrupção antecipada de tentativas.

- [ ] Escolher scoring e refit explicitamente.

- [ ] Avaliar trade-offs entre qualidade, memória e latência.

- [ ]  Registrar orçamento, espaço de busca e resultados completos.

- [ ]  Otimizar o pipeline, não somente o estimador.

- [ ]  Evitar tuning intenso antes de resolver problemas de dados e validação.

### Desbalanceamento e decisão

- [ ] Distinguir desbalanceamento de dificuldade real de separação.

- [ ] Comparar pesos de classe e pesos por amostra.

- [ ] Comparar oversampling e undersampling.

- [ ] Conhecer SMOTE, SMOTENC e métodos de limpeza.

- [ ] Investigar adequação da interpolação ao tipo de dado.

- [ ]  Aplicar reamostragem somente ao treino de cada fold.

- [ ]  Integrar reamostragem com pipelines do imbalanced-learn.

- [ ] Ajustar limiar segundo custo, recall mínimo ou capacidade operacional.

- [ ] Separar ajuste de limiar, calibração e treinamento.

- [ ] Avaliar consequências da prevalência diferente entre treino e operação.

- [ ]  Medir resultados na distribuição representativa do uso real.

### Calibração e incerteza

Um modelo calibrado que atribui probabilidade próxima de 0,8 deve apresentar aproximadamente 80% de positivos nesse conjunto de previsões. Isso é uma propriedade de grupos de previsões, não uma garantia sobre cada indivíduo.

- [ ] Diferenciar discriminação, calibração e decisão.

- [ ] Construir diagramas de confiabilidade.

- [ ] Usar CalibratedClassifierCV.

- [ ] Comparar calibração sigmoid e isotônica.

- [ ] Investigar limitações em amostras pequenas e classes raras.

- [ ]  Usar dados adequadamente separados para calibrar.

- [ ] Entender que Brier score e log loss não medem apenas calibração.

- [ ] Diferenciar previsão pontual, quantis e intervalos preditivos.

- [ ] Diferenciar incerteza epistemológica e aleatória.

- [ ] Conhecer conformal prediction como especialização.

- [ ]  Avaliar cobertura, largura e comportamento por segmento.

- [ ]  Definir critérios de abstinência ou encaminhamento humano quando necessário.

### Interpretabilidade e análise de erros

- [ ] Interpretar coeficientes considerando escala e codificação.

- [ ] Interpretar árvores e regras.

- [ ] Conhecer importância por redução de impureza.

- [ ] Investigar viés dessa importância e atributos correlacionados.

- [ ] Implementar importância por permutação.

- [ ] Interpretar PDP e ICE.

- [ ] Investigar extrapolações pouco plausíveis nas explicações.

- [ ] Conhecer SHAP e diferentes escolhas de referência.

- [ ] Distinguir explicações locais e globais.

- [ ] Avaliar estabilidade das explicações.

- [ ]  Não interpretar explicação preditiva como prova causal.

- [ ]  Categorizar erros e inspecionar exemplos representativos.

- [ ]  Analisar erros por segmento, faixa de score e período.

- [ ]  Priorizar novas ações a partir das falhas observadas.

### Texto no ML clássico

- [ ] Diferenciar documento, token e vocabulário.

- [ ] Implementar bag-of-words com CountVectorizer.

- [ ] Implementar TF-IDF.

- [ ] Comparar n-grams de palavras e caracteres.

- [ ] Controlar vocabulário com min_df, max_df e limites de atributos.

- [ ] Usar HashingVectorizer.

- [ ] Trabalhar com representações esparsas.

- [ ]  Construir pipelines de texto com modelos lineares ou Naive Bayes.

- [ ] Conhecer Latent Semantic Analysis e modelagem de tópicos.

- [ ] Diferenciar LDA de tópicos de LDA discriminante.

- [ ]  Evitar leakage por documentos repetidos e fontes compartilhadas.

### Aprendizado semissupervisionado e incremental

- [ ] Conhecer self-training e pseudo-labeling.

- [ ] Conhecer Label Propagation e Label Spreading.

- [ ] Investigar confirmação de erros e qualidade dos pseudo-rótulos.

- [ ] Diferenciar treinamento em lote e incremental.

- [ ] Usar partial_fit em estimadores compatíveis.

- [ ] Planejar atualização incremental do pré-processamento.

- [ ]  Processar dados em lotes sem carregar tudo na memória.

- [ ]  Preservar avaliação temporal e dados de teste durante atualizações.

### Reprodutibilidade e experimentação

- [ ] Registrar configurações, sementes e versões.

- [ ]  Versionar código, dados, atributos e artefatos.

- [ ]  Separar exploração de execução reproduzível.

- [ ]  Registrar hipóteses antes de grandes experimentos.

- [ ]  Manter tabela de comparação e histórico de decisões.

- [ ]  Reproduzir a execução em ambiente limpo.

- [ ]  Documentar métrica, divisão dos dados e limitações.

- [ ]  Evitar selecionar apenas resultados favoráveis.

### Produção e manutenção

A persistência deve considerar confiança na origem do artefato, dependências e compatibilidade. A documentação não oferece suporte geral a carregar modelos de uma versão diferente do Scikit-Learn.

- [ ]  Persistir pipeline, configuração e metadados.

- [ ]  Comparar joblib, pickle, skops.io e ONNX conforme a necessidade.

- [ ]  Não carregar artefatos pickle de fontes não confiáveis.

- [ ]  Fixar versões e reproduzir o ambiente de treinamento.

- [ ]  Definir contrato de entrada: nomes, tipos, unidades e campos obrigatórios.

- [ ]  Testar ausências, categorias novas e valores inválidos.

- [ ]  Testar consistência entre inferência individual e em lote.

- [ ]  Medir latência, throughput e memória.

- [ ]  Controlar paralelismo e evitar excesso de threads.

- [ ]  Monitorar qualidade de dados e distribuição das entradas.

- [ ]  Monitorar desempenho quando os rótulos estiverem disponíveis.

- [ ] Diferenciar data drift, mudança de prevalência e concept drift.

- [ ]  Definir critérios de retreinamento, substituição e rollback.

- [ ]  Documentar usos permitidos, limitações e responsáveis pelo modelo.

4. Especializações adicionais
Para o objetivo “Machine Learning em sentido amplo”, o núcleo anterior não encerra o currículo. Eu manteria os blocos abaixo como trilhas separadas, para que especializações não tornem o checklist principal uma barreira interminável.

Os dois primeiros blocos têm relação direta com áreas também apresentadas no guia do Scikit-Learn; causalidade e aprendizado por reforço constituem campos próprios, com conexões entre si.

### Aprendizado estatístico aprofundado

- [ ] Estudar generalização e complexidade de classes de hipóteses.

- [ ] Estudar regularização como escolha de viés indutivo.

- [ ] Investigar consistência, estabilidade e eficiência amostral.

- [ ] Estudar aprendizado bayesiano e predição posterior.

- [ ] Estudar métodos de covariância robusta e regularizada.

- [ ] Relacionar resultados teóricos às condições dos dados reais.

- [ ]  Reproduzir experimentos que evidenciem limites de generalização.

### Modelos probabilísticos

- [ ] Estudar modelos de mistura e o procedimento EM.

- [ ] Estudar modelos com variáveis latentes.

- [ ] Estudar redes bayesianas e modelos gráficos.

- [ ] Estudar Hidden Markov Models.

- [ ] Estudar inferência e aprendizagem de parâmetros nesses modelos.

- [ ]  Comparar modelos probabilísticos com alternativas discriminativas.

### Previsão temporal com ML

- [ ] Definir horizonte, frequência e disponibilidade dos atributos.

- [ ] Construir lags e janelas móveis sem acesso ao futuro.

- [ ] Criar baselines ingênuos e sazonais.

- [ ] Comparar previsão direta, recursiva e multi-horizonte.

- [ ] Estudar previsão global versus modelos por série.

- [ ]  Realizar backtesting compatível com a operação.

- [ ]  Avaliar por horizonte, série e período.

- [ ]  Tratar atrasos de atualização e variáveis externas indisponíveis.

### Recomendação e ranking

- [ ] Diferenciar recomendação, recuperação de candidatos e ranking.

- [ ] Implementar baselines de popularidade e conteúdo.

- [ ] Estudar filtragem colaborativa.

- [ ] Estudar fatoração de matrizes e feedback implícito.

- [ ] Diferenciar objetivos pointwise, pairwise e listwise.

- [ ] Estudar precision@k, recall@k, MAP, MRR e NDCG.

- [ ] Investigar cold start e viés de exposição.

- [ ]  Construir avaliação por usuário e por tempo.

### Sobrevivência e tempo até evento

- [ ] Diferenciar classificação de evento e previsão de tempo até evento.

- [ ] Reconhecer censura e seus efeitos sobre a modelagem.

- [ ] Estudar modelos de Cox e accelerated failure time.

- [ ] Estudar survival forests e boosting para sobrevivência.

- [ ] Conhecer riscos competitivos.

- [ ]  Avaliar discriminação e calibração ao longo do tempo.

### Causalidade e uplift

Causalidade exige distinguir associação de intervenção e explicitar as condições para inferir efeitos; não basta interpretar os atributos de um modelo preditivo.

- [ ] Diferenciar previsão de resultado e estimação de efeito.

- [ ] Identificar tratamento, resultado e confundidores.

- [ ] Estudar experimentos aleatorizados e suas limitações.

- [ ] Estudar identificação e hipóteses causais.

- [ ] Estudar métodos de propensity score e estimadores duplamente robustos.

- [ ] Estudar meta-learners de efeitos heterogêneos.

- [ ] Estudar causal forests e uplift modeling.

- [ ]  Documentar quais conclusões dependem de hipóteses não verificáveis.

### Aprendizado ativo e rótulos limitados

- [ ] Estudar seleção de exemplos por incerteza.

- [ ] Comparar incerteza, diversidade e estratégias por comitê.

- [ ] Estudar aprendizagem com rótulos fracos e positivos não rotulados.

- [ ] Investigar viés introduzido pela estratégia de aquisição.

- [ ]  Avaliar desempenho em função do orçamento de rotulagem.

- [ ]  Manter avaliação independente das amostras escolhidas para anotação.

### Robustez e transferência

- [ ] Diferenciar mudança de distribuição de erro de implementação.

- [ ] Estudar covariate shift, label shift e domain adaptation.

- [ ] Estudar aprendizado multitarefa e transferência.

- [ ] Investigar exemplos fora da distribuição.

- [ ] Estudar robustez a ruído, corrupção e manipulação de atributos.

- [ ]  Construir testes de estresse compatíveis com o contexto real.

### Aprendizado por reforço

Em RL, o objetivo é aprender uma política de interação que maximize um retorno, não apenas prever rótulos em um dataset estático.

- [ ] Identificar agente, ambiente, estado, ação e recompensa.

- [ ] Diferenciar retorno, valor de estado e valor de ação.

- [ ] Estudar exploração versus exploração do conhecimento adquirido.

- [ ] Estudar bandits e contextual bandits.

- [ ] Estudar métodos tabulares Monte Carlo e temporal difference.

- [ ] Estudar Q-learning e SARSA.

- [ ] Diferenciar métodos on-policy e off-policy.

- [ ] Estudar avaliação de políticas e aprendizado offline.

- [ ]  Avaliar segurança, custo de interação e qualidade da recompensa.

### Deep Learning

- [ ] Compreender a ponte entre MLPs e aprendizagem de representações.

- [ ] Estudar treinamento, regularização e diagnóstico de redes.

- [ ] Estudar arquiteturas para imagens, sequências, texto e grafos.

- [ ] Estudar transferência, autossupervisão e modelos generativos.

- [ ]  Manter um checklist próprio para implementação, treinamento e operação.

### Responsabilidade e governança

- [ ] Identificar grupos potencialmente prejudicados pelo sistema.

- [ ] Estudar diferentes critérios de fairness e seus trade-offs.

- [ ] Investigar riscos de privacidade e inferência de informação sensível.

- [ ]  Avaliar desempenho e erros por grupos relevantes.

- [ ]  Documentar origem dos dados, finalidade e limites de uso.

- [ ]  Definir supervisão humana, contestação e descontinuação do modelo.

Essas trilhas são um mapa de extensão. Não precisam ser concluídas antes de desenvolver projetos sólidos de ML tabular.

### 5. Evidências de domínio
Eu não marcaria um tópico como concluído apenas por conhecer sua definição. Para o seu objetivo de profundidade, adotaria estes critérios:

Explicar o tópico com suas próprias palavras, sem consultar material.

Implementar um exemplo mínimo e interpretar o resultado.

Mostrar uma situação em que o método falha.

Comparar com uma alternativa usando avaliação apropriada.

Registrar hipóteses, limitações e conclusão do experimento.