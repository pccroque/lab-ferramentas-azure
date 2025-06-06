# lab-ferramentas-azure

# Objetivo

Praticar e aprofundar o uso das ferramentas Azure Speech Studio e Language Studio, focando na análise de fala e linguagem natural. 
O objetivo é desenvolver habilidades práticas na criação de soluções baseadas em inteligência artificial voltadas para voz e linguagem. 

## Explorar o Speech no portal do Azure AI Foundry

### Criar um projeto no portal do Azure AI Foundry

1. No **portal do Azure AI Foundry**, entre com suas credenciais. 
	https://ai.azure.com
2. Em seguida, escolha a opção para **criar** um *novo recurso do hub de IA*.
	https://ai.azure.com/managementCenter/allResources
4. No *assistente Criar um projeto*, insira um nome válido para o projeto e, se um hub existente for sugerido, selecione a opção para *criar um novo*.
5. Expanda *Opções avançadas* para especificar as seguintes configurações para o projeto:
   * **Assinatura:** sua assinatura do Azure
   * **Grupo de recursos:** criar ou selecionar um grupo de recursos
   * **Região:** Selecione um dos seguintes locais:
      - Leste dos EUA
      - França Central
      - Coreia Central
      - Europa Ocidental
      - Oeste dos EUA<br>
Aguarde até que seu projeto e hub sejam criados.
6. Após a criação do projeto, será apresentado uma página de *Visão Geral* dos detalhes do projeto.
7. No menu à esquerda da tela, selecione **Playgrounds**.
8. Na página *Playgrounds*, selecione **Speech Playground** para experimentar alguns recursos do Azure AI Speech.

### Explorar a conversão de fala em texto no Speech Playground do Azure AI Foundry

Vamos experimentar a *conversão de fala em texto* no Speech Playground do Azure AI Foundry.

1. Na página Speech, role para baixo e selecione **Transcrição em tempo real** em *Experimentar recursos do Speech*. Você será levado ao *Speech Playground*.
2. Selecione https://aka.ms/mslearn-speech-files para baixar **speech.zip**. Abra a pasta.
3. Em *Carregar arquivos*, selecione **Procurar arquivos** e navegue até a pasta onde você salvou o arquivo. Selecione **WhatAICanDo.m4a** e, em seguida, **Abrir**.
4. O serviço de Fala transcreve e exibe o texto em tempo real. Se você tiver áudio em seu computador, poderá ouvir a gravação enquanto o texto está sendo transcrito.
5. Revise a saída, que deve ter reconhecido e transcrito com êxito o áudio em texto.<br>
   
Foi apresentado os serviços do Azure AI Speech no Speech Playground do Azure AI Foundry. Em seguida, foi usada a transcrição em tempo real para transcrever uma gravação de áudio. A transcrição do texto pode ser vista sendo gerada, enquanto o arquivo de áudio é resproduzido.

## Analisar texto no portal do Azure AI Foundry

### Criar um projeto no portal do Azure AI Foundry
*Da mesma forma do exemplo anterior.*

### Extrair entidades nomeadas com Azure AI Language no portal do Azure AI Foundry

*Entidades nomeadas* são palavras que descrevem pessoas, lugares e objetos com nomes próprios. Vamos usar a funcionalidade de extração de entidade nomeada do Azure AI Language para identificar tipos de informações em uma revisão.
1. No Language playground, selecione **Extrair informações**. Em seguida, selecione o bloco **Extrair entidades nomeadas**.
2. Em *Amostra*, copie e cole a seguinte revisão:

*Amostra*
```
Tired hotel with poor service
The Royal Hotel, London, United Kingdom
5/6/2018
This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk.
```

3. Selecione **Executar**. Revise a saída. Observe na seção *Detalhes* como as entidades extraídas vêm com informações adicionais, como pontuações de tipo e confiança. A pontuação de confiança representa a probabilidade de que o tipo identificado realmente pertença a essa categoria.
