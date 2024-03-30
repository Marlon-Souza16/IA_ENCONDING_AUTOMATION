# IA_ENCONDING_AUTOMATION

🔎 Problema Identificado

Este projeto foi desenvolvido com o objetivo de solucionar o problema encontrado no processo de codificação de descrições, que anteriormente era realizado manualmente. A necessidade de extrair códigos específicos de descrições era evidente, mas a execução manual desse processo consumia muito tempo e recursos humanos, podendo atrasar demais processos. 

✅ Solução

Para resolver esse problema, foi implementada uma solução baseada em inteligência artificial (IA) para automação da planilha. Utilizando a API da OpenAI para gerar sugestões de código com base nas descrições fornecidas. Para garantir a precisão da Api na hora de gerar os dados, foi implementado alguns tratamentos antes e após a requisição a api. Sendo assim o processo de codificação foi otimizado por meio de várias técnicas, incluindo o uso de expressões regulares para identificar padrões de código nas sugestões geradas, a formatação dos dados, removendo caracteres que não são importantes, tais quais virgulas, barras verticais, aspas e assim por diante, além de todo o texto ser colocado em Upper Case, e, após isso é  feito também a remoção de texto após palavras-chave específicas para evitar a obtenção de “falsos códigos” por parte da IA. 

Outro método implementado para garantir uma grande assertividade por parte da IA é utilizar exemplos dinâmicos de acordo com a descrição que queremos codificar, portanto, antes de enviarmos a prompt para api, buscamos na base vetorial os exemplos mais similares a essa descrição, aplicando a similaridade de cosseno nessa busca, assim, montando um prompt eficiente e específico para descrição que desejamos codificar.

Após obter uma sugestão de código, fazemos uma verificação para garantir que esse código obtido tenha sido extraído da descrição fornecida, assim, garantindo que o código seja verídico, e não um código “inventado” pela IA. Com essa verificação, tornamos o software ainda mais confiável e preciso na extração de códigos, assegurando a integridade dos resultados gerados. 


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

- [Python](https://www.python.org/doc/) (Linguagem de programação utilizada)
- [ChromaDB](https://docs.trychroma.com/usage-guide) (Base vetorial utilizada)
- [OpenAi](https://platform.openai.com/docs/api-reference/introduction) (Api utilizada)

🖊️ Autor

Marlon de Souza.
