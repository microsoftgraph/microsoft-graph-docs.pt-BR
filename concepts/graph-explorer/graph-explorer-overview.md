---
title: Usar o Explorador do Graph para tentar Microsoft Graph APIs
description: Use o Explorador do Graph para experimentar Microsoft Graph APIs no locatário de exemplo padrão para explorar os recursos ou entrar em seu próprio locatário e usá-lo como uma ferramenta de criação de protótipos para atender aos cenários do aplicativo.
ms.localizationpriority: high
author: RabebOthmani
ms.openlocfilehash: 56341c5b7efc0c6dcefcd5887f8003c613c7db01
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604221"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a>Usar o Explorador do Graph para tentar Microsoft Graph APIs

[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) é uma ferramenta de desenvolvedor que permite que você faça convenientemente Microsoft Graph solicitações da API REST e exiba as respostas correspondentes. Use o Explorador do Graph para experimentar APIs no locatário de exemplo padrão para explorar os recursos ou entrar em seu próprio locatário e usá-lo como uma ferramenta de criação de protótipos para atender aos cenários do aplicativo. Essa ferramenta inclui recursos úteis, como snippets de código em C#, Java, JavaScript e Objective C; Microsoft Graph integração de kit de ferramentas e cartões adaptáveis; e muito mais.

Use o Explorador do Graph para:

- Faça Microsoft Graph de API (GET, POST, PUT, PATCH e DELETE) e veja respostas, incluindo código de resposta e quaisquer cabeçalhos e corpos.
- Consentimento para permissões. O Graph Explorer dá suporte apenas [permissões delegadas](/graph/auth/auth-concepts#delegated-and-application-permissions).
- Adicione um corpo de solicitação e um cabeçalho de solicitação à sua consulta.
- Exiba e copie o token de acesso.
- Exiba consultas de exemplo para diferentes serviços no Microsoft Graph.
- Exiba, baixe ou exclua as consultas que você executou nos últimos 30 dias.
- Exiba e copie snippets de código de cada consulta executada em C#, Java, JavaScript e Objective C.
- Acesse Microsoft Graph componentes do Kit de Ferramentas e cartões adaptáveis para algumas consultas de exemplo.
- Compartilhe consultas, incluindo o corpo da solicitação e os cabeçalhos de solicitação.

O Explorador do Graph lida com o processo de autenticação para você. Personalize a experiência ao recolher a barra lateral ou alterar o tema.

## <a name="get-started"></a>Introdução

Graph Explorer é um aplicativo da web hospedado no [centro de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/en-us/graph/graph-explorer). É um projeto de código aberto e agradecemos suas contribuições e comentários no [repositório GitHub](https://github.com/microsoftgraph/microsoft-graph-explorer-v4).

O Explorador do Graph inclui os seguintes elementos:

1. Lista suspensa de verbos HTTP
2. Lista suspensa de versão da API
3. Solicitar barra de endereços de consulta
4. Consulta de exemplo
5. Link de documentação para a consulta de exemplo

:::image type="content" source="./images/getting-started.png" alt-text="Captura de tela da interface de usuário do Graph Explorer" border="true":::.

### <a name="make-a-get-request-in-graph-explorer"></a>Fazer uma solicitação GET no Graph Explorer

Para executar uma solicitação GET no Graph Explorer, você não precisa estar conectado. Basta clicar em uma consulta de exemplo e os dados de exemplo serão mostrados na visualização da resposta. 

:::image type="content" source="./images/making-a-get-request.png" alt-text="Captura de tela de uma solicitação de exemplo no Explorador do Graph." border="true":::

Para fazer uma solicitação:

1. Selecione uma consulta de exemplo e execute-a.
2. Obtenha o código de resposta HTTP.
3. Consulte a resposta da API de Microsoft Graph com dados de exemplo.

Quando você entrar no Explorador do Graph e clicar na mesma consulta, a resposta será retornada com dados reais do locatário ao qual você entrou.

### <a name="running-non-get-requests-in-graph-explorer"></a>Executando solicitações não GET no Graph Explorer

Para experimentar as solicitações POST, PUT, PATCH e DELETE, entre no Graph Explorer usando uma Microsoft 365 conta. Pode ser uma conta organizacional para fins de teste ou demonstração. Para obter uma amostra grátis de assinatura de desenvolvedor do Microsoft 365 E5, junto com ferramentas e outros recursos para ajudá-lo a criar soluções para a plataforma Microsoft 365, associe-se ao [Programa de Desenvolvedor do Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program). 

>[!IMPORTANT]
>Se você optar por entrar usando sua conta organizacional, executar uma solicitação não GET poderá afetar os dados no locatário.

Por exemplo, para executar uma solicitação POST, selecione POST na lista suspensa para o verbo HTTP e adicione um corpo de solicitação e cabeçalhos de solicitação conforme apropriado.

:::image type="content" source="./images/making-a-post-request.png" alt-text="Captura de tela de uma solicitação POST no Explorador do Graph." border="true":::

1. Selecione uma consulta de exemplo POST.
2. Atualizar **Corpo da solicitação;** por exemplo, dê um nome ao aplicativo.
3. Clique em **Executar consulta**.
4. Consulte a resposta da API do Microsoft Graph.

Para exibir a resposta em um formato diferente do JSON padrão, escolha a guia **Cabeçalhos** de solicitação no painel de solicitação, defina o par chave/valor e clique em **Adicionar**.

:::image type="content" source="./images/adding-key-value-pairs.png" alt-text="Captura de tela que mostra a guia de Cabeçalhos de solicitação no Explorador do Graph." border="true":::

## <a name="next-steps"></a>Próximas etapas

- Visite o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/).
- Saiba mais sobre o [Explorador do Graph](./graph-explorer-features.md).
- Contribua ou forneça comentários no [repositório do GitHub](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).
