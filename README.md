# google-data-analytics-bellabeat-casestudy
Estudo de Caso Bellabeat - Projeto de Conclusão Google Data Analytics
As 6 Fases do Processo de Análise de Dados
Este projeto seguiu as seis fases do processo de análise de dados para garantir uma abordagem estruturada, desde a definição do problema de negócio até a entrega de recomendações estratégicas.

1. Fase de Perguntar (Ask)
O projeto iniciou com uma clara tarefa de negócio solicitada pela liderança da Bellabeat: analisar dados de uso de dispositivos de fitness para identificar tendências e, com base nelas, propor novas estratégias de marketing para impulsionar o crescimento da empresa. O objetivo principal era transformar dados brutos em insights acionáveis para o negócio.

2. Fase de Preparar (Prepare)
Nesta fase, utilizamos um conjunto de dados públicos do Kaggle (Fitbit Fitness Tracker Data) contendo dados de 33 usuários. A preparação envolveu uma análise crítica da fonte de dados, onde identificamos suas principais forças (granularidade dos dados) e fraquezas, como o tamanho limitado da amostra e o fato de os dados serem de 2016. Essa avaliação inicial foi crucial para contextualizar as futuras descobertas.

3. Fase de Processar (Process)
Esta foi a fase tecnicamente mais desafiadora. Os dados foram carregados no Google BigQuery para processamento com SQL. Enfrentei e solucionei diversos problemas de importação, incluindo inconsistências nos delimitadores dos arquivos CSV (alguns usavam vírgulas, outros ponto e vírgula) e erros de detecção de tipo de dados. A solução envolveu a definição manual do esquema das tabelas, garantindo a integridade e a correta estruturação dos dados para a análise. Também realizei a limpeza e formatação das colunas de data, convertendo-as de STRING para TIMESTAMP para permitir análises temporais.

4. Fase de Analisar (Analyze)
Com os dados limpos, a análise focou em descobrir padrões de comportamento. A primeira grande descoberta foi que os usuários passavam, em média, mais de 16 horas por dia em estado sedentário. Investiguei a hipótese de que isso seria um erro de medição (ex: usuários não usando o dispositivo 24h), mas os dados provaram que o tempo de uso era integral. Aprofundando a análise com um JOIN entre dados de atividade e sono, descobri o insight principal: mesmo subtraindo as ~7 horas de sono, restavam quase 5 horas de inatividade durante o dia. Além disso, confirmei uma forte correlação positiva entre o total de passos e as calorias queimadas.

5. Fase de Compartilhar (Share)
Para comunicar as descobertas de forma eficaz, conectei o BigQuery ao Looker Studio e criei um dashboard visual. As visualizações incluíram:

Cartões de Pontuação para destacar a distribuição média de minutos por tipo de atividade.

Um Gráfico de Dispersão para ilustrar a relação entre passos e calorias.

Um Gráfico de Barras Comparativo para mostrar a diferença entre o tempo de sono e o tempo sedentário acordado.
Esses visuais foram essenciais para contar a história dos dados de forma clara e impactante.

6. Fase de Agir (Act)
A fase final consistiu em traduzir os insights em estratégia de negócio. Com base nas descobertas, elaborei três recomendações estratégicas para a Bellabeat:

"Jornada de Bem-Estar Ativo": Uma funcionalidade no app para combater o sedentarismo diário com notificações inteligentes.

"Assistente de Sono Premium": Uma evolução da funcionalidade de sono para impulsionar o serviço de assinatura.

"Comunidade Bellabeat": Uma plataforma de engajamento para educar sobre as funcionalidades e fortalecer a marca.

Cada recomendação foi diretamente embasada nos dados e focada em gerar valor tanto para o usuário quanto para a empresa.
