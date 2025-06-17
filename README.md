# Projeto de Modelagem de Dados com Estrutura Medalhão e Dashboard Power BI

Este projeto é uma releitura do meu principal trabalho da época em que fui estagiário na área de siderurgia.  
Naquele momento, fui responsável pela criação de aplicativos para registrar não conformidades em cargas de matéria-prima (sucata).  
Por estar no início da minha carreira, não sabia exatamente como transformar esses dados em decisões estratégicas.

Hoje, buscando me aperfeiçoar em análise e engenharia de dados, resolvi reformular esse projeto para aplicar boas práticas e criar uma solução que entregue insights claros e úteis para o negócio.

## Contexto do Projeto

Os dados foram modelados no Databricks seguindo a arquitetura medalhão, utilizando três tabelas fictícias para representar o fluxo de informações.  
A estrutura medalhão foi adotada para organizar os dados em camadas de qualidade e confiabilidade, facilitando a análise e a visualização.

Além disso, foi desenvolvido um dashboard em Power BI para dar suporte visual e interativo às decisões.

## Principais questões que o projeto busca responder

- **Qual fornecedor apresenta mais não conformidade de carga?**  
  Com detalhamento por tipo de não conformidade e material.

- **Qual horário do dia costuma apresentar maior concentração de cargas não conformes?**

- **Qual turno apresenta maior registro de não conformidades?**

## Estrutura do Projeto

- `/databricks`  
  Contém notebooks e scripts SQL usados para criação e transformação das tabelas (camadas Bronze, Silver e Gold).

- `/powerbi`  
  Arquivo do dashboard Power BI (`.pbix`) para visualização dos dados finais.

- `/docs`  
  Documentação complementar e instruções.

## Arquitetura Medalhão

- **Bronze**: Dados crus, coletados diretamente da fonte, sem tratamento.  
- **Silver**: Dados limpos e filtrados, prontos para análises intermediárias.  
- **Gold**: Dados agregados e otimizados para relatórios e dashboards.

## Como usar

1. Importe os notebooks da pasta `/databricks` no workspace Databricks.  
2. Execute os notebooks na sequência Bronze → Silver → Gold para criar as tabelas transformadas.  
3. Abra o arquivo Power BI na pasta `/powerbi` para visualizar o dashboard interativo.

## Considerações

- As tabelas são fictícias e usadas para fins educacionais e demonstração.  
- O projeto pode ser adaptado para dados reais e ampliado conforme necessidade.
