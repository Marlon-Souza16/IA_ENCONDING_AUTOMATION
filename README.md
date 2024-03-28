# IA_ENCONDING_AUTOMATION

🔎 Problema Identificado

Este projeto foi desenvolvido com o objetivo de solucionar o problema encontrado no processo de codificação de descrições, que anteriormente era realizado manualmente. A necessidade de extrair códigos específicos de descrições era evidente, mas a execução manual desse processo consumia muito tempo e recursos humanos, podendo atrasar demais processos. 

✅ Solução



📚 Bibliotecas Necessárias

- OpenAi (Api utilizada para encontrar as sugestões de código)
- ChromaDB (Base de dados vetorial utilizada para guardar os exemplos utilizados pela API)
- Time (Para calcular o tempo de execução da Api e de cada requisição)
- Panda (Utilizado para carregar, manipular e salvar os dados)
- Glob (Utilizada para procurar todos os arquivos csv intermediários gerados)
- Os (Utilizada para manipular arquivos, incluindo a verificação da existência de arquivos e a exclusão de arquivos intermediários após o processamento)
- Re (Utilizada para lidar com expressões regulares)
- csv (Utilizada para lidar com arquivos CSV)
- Unidecode (Utilizada para realizar a remoção de caracteres com acento das descrições)
- Tenacity (Utilizada para em caso de erro aplicar um retry a função desejada)

📋 Pré-requisitos

- Instalar o python
- Instalar a OpenAi
- Instalar o ChromaDB
- E as demais bibliotecas listadas acima

🔧 Instalação

- Comando para instalar a Api da OpenAi: ```pip install openai```
- Comando para instalar o ChromaDB: ```pip install chromadb```

🛠️ Construído com

- [Python](https://www.python.org/doc/) (Linguagem de programação utilziada)
- [ChromaDB](https://docs.trychroma.com/usage-guide) (Base vetorial utilizada)
- [OpenAi](https://platform.openai.com/docs/api-reference/introduction) (Api utilizada)

🖊️ Autor

Marlon de Souza.
