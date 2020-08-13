# MineracaoDadosEnemTeresina

Feito com Jupyter Notebook e a ferramenta Orange

Primeiro Precisa baixar a base dos microdados do ENEM em http://inep.gov.br/microdados

Atualizar a localização do arquivo na variável path do notebook Leitura Microdados Enem 

A partir daí executar os notebooks na seguinte ordem:

1. Leitura Microdados Enem 
1. TratandoDadosEnem
1. TratandoDadosEnem_Apriori
1. Clusterização
1. Resultados

Para gerar as regras de associação, usar o programa Orange na base resultante da clusterização (agrupadas_notas_normalizadoQuantil.csv)

1. Abrir no programa Orange o workflow AnaliseCluster_NOTAS
1. Carregar o  arquivo agrupadas_notas_normalizadoQuantil.csv
1. Abrir o widget Association Rules:
   - Definir os parâmetros:
   - Support: 20%
   - Confidence: 70%

   (esses foram os valores usados para o artigo, pode mudar conforme desejar) 



