
# Projeto-05-AI900
## IA Gerativa
### Objetivo: Criar um ambiente no Azure para uso do serviço Azure OpenAI, possibilitando o acesso a modelos generativos de IA desenvolvidos pela OpenAI. Implementar um modelo específico (gpt-35-turbo) no Azure OpenAI Studio para gerar conteúdo em linguagem natural, demonstrando a capacidade de utilizar modelos de IA em cenários de interação textual. Entender e experimentar os filtros de conteúdo padrão do Azure OpenAI, bem como a possibilidade de criar filtros personalizados, visando garantir a aplicação de princípios de IA responsável e segura em interações geradas pela IA.

Passo a passo está na documentação oficial da Microsoft:

[Explore o Microsoft Copilot no Microsoft Edge](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/12-generative-ai.html)

[Explore o Azure OpenAI](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/13-azure-openai.html)

[Explore content filters in Azure OpenAI](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/14-azure-openai-content-filters.html)


Explore a IA generativa com o Microsoft Copilot

1. Preparação
* Instale o Microsoft Edge: Se ainda não tiver o Microsoft Edge instalado, baixe e instale-o gratuitamente em https://www.microsoft.com/edge/download.
* Crie uma conta da Microsoft: Se ainda não tiver uma conta da Microsoft, inscreva-se em https://signup.live.com.
Faça login no Microsoft Edge: Use sua conta da Microsoft para fazer login no Microsoft Edge.

2.  Acesso ao OneDrive e Documento
* Acesse o OneDrive: Navegue até o OneDrive em https://onedrive.live.com e faça login usando sua conta da Microsoft.
* Baixe o Documento: Abra o documento Business Idea.docx em https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/raw/main/data/generative-ai/Business%20Idea.docx e salve-o na pasta Documentos do OneDrive.

3. Uso do Copilot
* Ative o Copilot: No Microsoft Edge, clique no ícone do Copilot na barra de ferramentas para abrir o painel Copilot.
* Interaja com o Copilot:
    * Faça perguntas como "What is this document about?", "What's the market opportunity for this business idea?", e "How do I go about setting up a business in New York?" para obter insights e orientações.
    * Siga as respostas do Copilot para desenvolver um plano de negócios, criar um nome para sua empresa, gerar um logotipo corporativo e até mesmo redigir um e-mail para investidores.

4. Criação de um Plano de Negócios e Apresentação
* Escreva o Plano de Negócios: Use as respostas do Copilot para escrever o plano de negócios para sua empresa de limpeza.
* Crie uma Apresentação: Use o PowerPoint para criar uma apresentação com base nos insights gerados pelo Copilot.

5. Redação de um E-mail
* Inicie o Outlook: Use o Iniciador de Aplicativos no OneDrive para abrir o Outlook.(nesse caso usei meu G-mail)
* Redija o E-mail: Componha um e-mail para investidores com a ajuda do Copilot para gerar o conteúdo.

* Desafio Opcional
    * Tente explorar mais o Copilot em uma nova sessão para planejar um evento de promoção da alfabetização infantil em uma biblioteca local.
    * Siga esses passos para explorar o Microsoft Copilot no Microsoft Edge conforme solicitado. Se precisar de mais detalhes em algum dos passos, fique à vontade para pedir mais orientações.


1. Provisão do Recurso Azure OpenAI
* Acesso ao Portal do Azure: Acesse o Portal do Azure.
* Criação do Recurso Azure OpenAI:
    * Selecione "Criar um recurso" no menu do portal.
    * Procure por "Azure OpenAI" e selecione o serviço.
    * Escolha sua assinatura do Azure e o grupo de recursos existente ou crie um novo.
    * Na configuração do recurso, defina a região como Leste dos EUA, o nome exclusivo de sua escolha e o nível de preços como Padrão S0.
    * Aguarde a conclusão da implantação e acesse o recurso Azure OpenAI no portal do Azure.

2. Exploração do Azure OpenAI Studio
* Acesso ao Azure OpenAI Studio:
    * Na página Visão Geral do recurso Azure OpenAI, clique em "Explorar" para abrir o Azure OpenAI Studio em um novo separador do navegador.
    * Se preferir, você pode navegar diretamente para o Azure OpenAI Studio.
* Exploração das Páginas Disponíveis:
    * No Azure OpenAI Studio, você verá diversas páginas no painel esquerdo, como Modelos, Implantações, Playground do Chat e Playground DALL-E.

3. Implantação de um Modelo de Geração de Texto
* Seleção e Implantação do Modelo:
    * Na página Modelos, escolha um modelo gpt-35-turbo com status "Implantável" como Sim e clique em "Implantar".
    * Configure a nova implantação com as opções necessárias, como nome exclusivo, versão do modelo, filtro de conteúdo, tipo de implantação e limite de taxa de tokens por minuto.
* Uso do Playground do Chat:
    * Navegue até o playground do Chat no painel esquerdo do Azure OpenAI Studio.
    * Certifique-se de que a implantação do seu modelo esteja selecionada.
    * Envie mensagens de usuário para interagir com o modelo e receber respostas em linguagem natural.

4. Geração de Imagens com DALL-E
* Acesso ao Playground DALL-E:
    * No Azure OpenAI Studio, vá para o playground DALL-E no painel esquerdo.
    * Insira prompts para gerar imagens com base nas descrições fornecidas.
    * Explore diferentes prompts e visualize as imagens geradas pelo modelo DALL-E.


1. Provisionar um Recurso Azure OpenAI
* Acesse o Portal do Azure e crie um recurso Azure OpenAI com as seguintes configurações:
    * Assinatura: Sua assinatura do Azure aprovada para acesso ao serviço Azure OpenAI.
    * Grupo de recursos: Escolha um existente ou crie um novo com um nome de sua escolha.
    * Região: Escolha aleatoriamente uma das seguintes regiões:
        * Australia East
        * Canada East
        * East US
        * East US 2
        * France Central
        * Japan East
        * North Central US
        * Sweden Central
        * Switzerland North
        * UK South
    * Nome: Um nome exclusivo de sua escolha.
    * Nível de preços: Padrão S0.

2. Implantação de um Modelo
* Acesse o Azure OpenAI Studio:
    * Na página Visão Geral do seu recurso Azure OpenAI, clique em "Explorar" para abrir o Azure OpenAI Studio em uma nova guia do navegador. Alternativamente, acesse diretamente o Azure OpenAI Studio.
* Crie uma Nova Implantação:
    * No Azure OpenAI Studio, crie uma nova implantação com as seguintes configurações:
        * Modelo: gpt-35-turbo
        * Versão do modelo: Atualização automática para padrão
        * Nome da implantação: Um nome exclusivo de sua escolha.
        * Opções avançadas:
            * Filtro de conteúdo: Padrão
            * Tipo de implantação: Padrão
            * Limite de taxa de tokens por minuto: 5K (ou outro valor adequado)
            * Habilitar cota dinâmica: Habilitado
3. Gerar Saída em Linguagem Natural
* No Playground do Chat:
    * Navegue até o playground do Chat no Azure OpenAI Studio.
    * Selecione o modelo implantado em suas configurações.
    * No painel de sessão de chat, envie prompts para gerar saída em linguagem natural.

4. Explorar Filtros de Conteúdo
* Página de Filtros de Conteúdo:
    * No Azure OpenAI Studio, vá para a página de Filtros de Conteúdo.
    * Selecione "Criar filtro de conteúdo personalizado" para revisar as configurações padrão e personalizadas dos filtros de conteúdo.

5. Limpeza
Quando terminar, lembre-se de limpar os recursos no portal Azure para evitar custos adicionais. Você pode remover a implantação específica ou todo o recurso Azure OpenAI, conforme necessário.
