Piloto VODAN BR
+++++++++++++++
	
O piloto do projeto VODAN BR tem por objetivo aprofundar os conhecimentos em workflows de FAIRificação e na tecnologia do FAIR DP; e analisar e selecionar as ferramentas necessárias para a infraestrutura proposta. O piloto atua em uma plataforma simplificada, empregando datasets sobre pacientes com COVID, disponibilizados pelo repositório COVID-19 DataSharing/BR . Esse repositório é uma iniciativa da FAPESP em cooperação com a Universidade de São Paulo, e, inicialmente, participação do Instituto Fleury, Hospital Sírio-Libanês (HSL) e Hospital Israelita Albert Einstein, com o objetivo de disponibilizar dados relacionadas à COVID-19 que possam contribuir para pesquisas desta temática.

Para o piloto foram empregados, especificamente, os dados disponibilizados pelo HSL. Uma análise de seus dados permitiu identificar a existência de informações associadas à admissão, ao acompanhamento e ao desfecho dos pacientes atendidos. Esses dados foram tratados e transformados, conforme previsto na RI VODAN, para atender ao formato do Case Record Form (CRF) estabelecido pela Organização Mundial de Saúde para registro de dados sobre a COVID-19.

Um Workflow de FAIRificação foi desenvolvido, estabelecendo um conjunto de ações para as fases/etapas, a partir de um workflow genérico original apresentado em [5]. Essas ações foram analisadas e validadas no processo de transformação de dados e metadados do Piloto.

A Figura 1 apresenta uma visão esquematizada do Piloto e das etapas referentes ao Workflow. Nessa figura, a plataforma captura conjuntos de dados de pacientes COVID-19, em formato CSV (1), aplicando as etapas da fase de pré-FAIRificação (a). Este conjunto de dados e os resultados das análises realizadas são utilizados nas etapas 4a e 4b da fase de FAIRificação (b), estabelecendo os modelos semânticos para dados e metadados. Seguindo as ações especificadas nas etapas 5a e 5b, o processo Extração, Transformação e Carga (ETL), designado como ETL4FAIR (2), é responsável por transformar os dados e metadados para a representação RDF. Após a transformação, segue-se a etapa 6, responsável pela hospedagem dos dados e metadados em uma triplestore (3), com os esquemas de metadados referentes ao dataset e sua distribuição publicados no FAIR DP (5). Na etapa 7, na fase denominada pós-FAIRificação (c), o Workflow promove a avaliação do nível de maturidade FAIR atribuído aos dados e metadados, e a validação da plataforma estabelecida.

 .. image:: images/Plataforma_Piloto_VODANBR.png
 Figura 1 – Visão Simplificada da Plataforma do Piloto VODAN BR associado as Etapas de FAIRificação


Uma versão preliminar dos dados e metadados foi gerada e publicada usando o GraphDB e FAIR DP. Novas discussões estão sendo realizadas para se aprimorar os modelos semânticos para proveniência a serem adotados no piloto e, futuramente, no projeto.
