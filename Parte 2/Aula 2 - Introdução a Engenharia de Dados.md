# Qual o papel de engenheiro de dados

O aumento da quantidade de dados disponíveis e a demanda por cientistas de dados para analise-los fez com que a profissão de engenheiro de dados se tornasse essencial para as organizações.

Possui habilidades relacionadas ao desenvolvimento e arquitetura de software, além de sólidos conhecimentos em banco de dados, DevOps e infraestrutura de TI.

## Definição

>"Engenheiro de Dados é um tipo especializado de Engenheiro de Software que possibilita outros a responderem questões sobre grandes Datasets com restrições específicas de latência e tempo."

## Resposabilidade

> Garantir que os dados estejam disponível para analise de forma segura.

Nº | Etapa  | Procedimentos |
---|--------|------------|
01 | Coleta |Jobs(batch) e Realtime(streaming) | 
02 | Transoformação | ETL e Pipelines |
03 | Armazenamento | Banco de dados e Repositórios de arquivos |
04 | Disponibilidade | API's, Arquivos e Banco de dados |

## BI - Business Itelligence

> Converter o volume de dados em informações relevantes para o negócios, por meio de relatórios analíticos.

**Aplicações**
- Query Report
- Mineração de dados
- Budget & Forecast
- KPI's
- Dashboards de Gestão

**Ferramentas**

- MicroStrategy
- Google Data Studio
- Looker
- Microsoft Power BI
- Tableau
- QlikView
- Board

## Data Warehouse

- Falta de credibilidade dos dados, consequência de extrações.
- Baixa Produtividade.
- Dificuldade em gerar informação a partir dos dados extraídos.

**Definição**

É uma arquitetura de armazenamento projetada para conter dados extraídos de sistemas de transções, armazenamentos de dados operacionais e fontes externas.

Combina esses dados em um formulário de resumo agregado adequado para análise de dados em toda a empresa e relatórios para necessidades de negócios predefinidas.

## OLTP vs OLAP

Etapas | OLTP | OLAP |
--------|---------|-------|
Foco| Operações do dia a dia | Suporte a decisão |
Origem| Transações em tempo real da organização | Base de dados de sistemas transacionais |
Performance| Milissegundos | Minutos/Horas |
Volatilidade| Atualizações curtas e rápidas iniciadas pelo usuário | Geralmente grande devido à agregação de grandes conjuntos de dados |
Design| Normalizado | Desnormalizado |

## Movimentação de Dados

**ETL**:(Extract, Transform, Load) é um processo automatizado que coleta dados brutos, extrai as informações necessárias para analise, transforma em formato que atende às necessidades de negócios e carrega em um data warehouse.

- Movimentação de volumes de dados.
    - Cargas completas - truncate & load.
    - Cargas incrementais- data / ID.
    - Frequência (diária, semanal, mensal).

- Pode melhorar significativamente a qualidade dos dados.
    - Qualidade e padronização/validação dos dados.
    - Metadados (descrevem os atributos dos dados - significado)

**ETL - Desafios**

- Escalabilidade - A escalabilidade é um dos recursos mais importantes em uma ferramenta ETL moderna.

- Acurácia - garantir que os dados que você transforma sejam precisos e completos.

- Manusear fontes de dados diversas - lidar com diversos tipos de fontes de dados.

**Considerações finais**

- DW é fundamental para um sistema de apoio à decisão.
- Acesso simplificado a dados historicos.
- Facilidade em consulta de informações.
- Avalie as origens e tipos de dados.
- Planeje a malha de ETLs.
- Atenção a modelagem dos dados(Dimensional).
- Produção de relatórios.

## Data Marts

 É um subconjunto de um data warehouse.
  
 Orientado para uma única linha de negócio específica.
  
 Contêm repositórios de dados resumidos coletados para análise em uma seção ou unidade específica dentro de uma organização.
  
 ... Por exemplo, o departamento de vendas.