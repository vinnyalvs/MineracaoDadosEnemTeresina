# MineracaoDadosEnemTeresina

Feito com Jupyter Notebook e a ferramenta Orange

# Objetivos

### Estudo de caso sobre Estudantes do último ano do Ensino Médio da cidade de Teresina Piaui

# Metodologia:
1. Limpeza e tratamento de dados
1. Aplicação de algoritmo de clusterização Kmeans com Sci-kit Learn
1. Aplicação de algoritmo de mineração de regras de associação com Orange ou bilioteca apyori

# Como executar

Primeiro Precisa baixar a base dos microdados do ENEM em http://inep.gov.br/microdados

Atualizar a localização do arquivo na variável path do notebook Leitura Microdados Enem 

1. Criar pasta Dados
1. Criar pasta Gráficos

A partir daí executar os notebooks na seguinte ordem:

1. Leitura Microdados Enem 
1. TratandoDadosEnem
1. TratandoDadosEnem_Apriori
1. Clusterização
1. Resultados (é possível executar esse Jupyter diretamente pois o arquivo agrupadas_notas_normalizadoQuantil.csv esta versionado)

Para gerar as regras de associação, usar o programa Orange na base resultante da clusterização (agrupadas_notas_normalizadoQuantil.csv)

1. Abrir no programa Orange o workflow AnaliseCluster_NOTAS
1. Carregar o  arquivo agrupadas_notas_normalizadoQuantil.csv
1. Abrir o widget Association Rules:
   - Definir os parâmetros:
   - Support: 20%
   - Confidence: 70%

   (esses foram os valores usados para o artigo, pode mudar conforme desejar) 



