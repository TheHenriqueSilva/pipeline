Pipeline de Processamento de Dados
Este repositório contém um pipeline ETL (Extract, Transform, Load) em Python, projetado para ler dados de diferentes formatos (JSON e CSV), transformá-los e, em seguida, consolidá-los em um único arquivo CSV.

🚀 Funcionalidades
Extração de Dados: Lê dados de arquivos JSON e CSV de forma eficiente.

Transformação de Dados:

Renomeia colunas para padronização.

Combina dados de múltiplas fontes (JSON e CSV) em uma única estrutura.

Carregamento de Dados: Salva os dados processados em um novo arquivo CSV.

📁 Estrutura do Projeto
processamento_dados.py: Contém a classe Dados responsável pelas operações de leitura, transformação e salvamento de dados.

main.py (ou nome similar para o script principal): Orquestra o pipeline, chamando as funções da classe Dados para executar as etapas de ETL.

data_raw/: Diretório para armazenar os arquivos de dados brutos de entrada (ex: dados_empresaA.json, dados_empresaB.csv).

data_process/: Diretório para armazenar os arquivos de dados processados (ex: dados_combinados.csv).

🛠️ Como Usar
Pré-requisitos
Certifique-se de ter o Python 3 instalado em seu ambiente.

Instalação
Não há bibliotecas externas complexas. Apenas as bibliotecas padrão json e csv do Python são utilizadas.

Execução
Clone o repositório:

Bash

git clone https://github.com/TheHenriqueSilva/pipeline.git
cd pipeline
Organize seus dados brutos:
Crie a pasta data_raw na raiz do projeto e coloque seus arquivos dados_empresaA.json e dados_empresaB.csv (ou os nomes que você usa) dentro dela.

Execute o pipeline:

Bash

python main.py # ou o nome do seu arquivo principal
Após a execução, o arquivo dados_combinados.csv será gerado na pasta data_process/.

💡 Como Funciona
O pipeline segue as seguintes etapas:

Extract (Extração):

Lê dados_empresaA.json usando a classe Dados com o tipo json.

Lê dados_empresaB.csv usando a classe Dados com o tipo csv.

Transform (Transformação):

As colunas de dados_empresaB são renomeadas para padronizar os nomes com os de dados_empresaA.

Os dados das duas empresas são combinados em uma única estrutura.

Load (Carregamento):

Os dados combinados são salvos no arquivo data_process/dados_combinados.csv.

🤝 Contribuições
Sinta-se à vontade para abrir issues ou pull requests se tiver sugestões de melhorias ou encontrar algum bug.

