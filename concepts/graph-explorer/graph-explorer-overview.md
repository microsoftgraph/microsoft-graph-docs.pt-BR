---
title: Usar o Explorador do Graph para tentar Microsoft Graph APIs
description: Use o Explorador do Graph para experimentar Microsoft Graph APIs no locatário de exemplo padrão para explorar os recursos ou entrar em seu próprio locatário e usá-lo como uma ferramenta de criação de protótipos para atender aos cenários do aplicativo.
ms.localizationpriority: high
author: RabebOthmani
ms.openlocfilehash: 9f1d112cc47493b36fe455d817aa637e7fda783e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176592"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a>Usar o Explorador do Graph para tentar Microsoft Graph APIs

[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) é uma ferramenta de desenvolvedor que permite que você faça convenientemente Microsoft Graph solicitações da API REST e exiba as respostas correspondentes. Use o Explorador do Graph para experimentar APIs no locatário de exemplo padrão para explorar os recursos ou entrar em seu próprio locatário e usá-lo como uma ferramenta de criação de protótipos para atender aos cenários do aplicativo. Essa ferramenta inclui recursos úteis, como trechos de código (C#, Java e JavaScript), Kit de ferramentas do Microsoft Graph e integração de cartões adaptáveis e muito mais.

Use o Explorador do Graph para:

- Faça solicitações de API do Microsoft Graph (GET, POST, PUT, PATCH e DELETE) e veja as respostas, incluindo o código de resposta e quaisquer cabeçalhos e corpos.
- Consentimento para permissões. O Graph Explorer dá suporte apenas [permissões delegadas](/graph/auth/auth-concepts#delegated-and-application-permissions).
- Adicione um corpo de solicitação e um cabeçalho de solicitação à sua consulta.
- Exiba e copie o token de acesso.
- Exiba consultas de exemplo para diferentes serviços no Microsoft Graph.
- Exiba, baixe ou exclua as consultas que você executou nos últimos 30 dias.
- Exiba e copie trechos de código de cada consulta executada em C#, Java e JavaScript.
- Acesse Microsoft Graph componentes do Kit de Ferramentas e cartões adaptáveis para algumas consultas de exemplo.
- Compartilhe consultas, incluindo o corpo da solicitação e os cabeçalhos de solicitação.

O Explorador do Graph lida com o processo de autenticação para você. Personalize a experiência ao recolher a barra lateral ou alterar o tema.

## <a name="get-started"></a>Introdução

Graph Explorer é um aplicativo da web hospedado no [centro de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/en-us/graph). É um projeto de código aberto e agradecemos suas contribuições e comentários no [repositório GitHub](https://github.com/microsoftgraph/microsoft-graph-explorer-v4).

O Explorador do Graph inclui os seguintes elementos:

1. Lista suspensa de verbos HTTP
2. Lista suspensa de versão da API
3. Solicitar barra de endereços de consulta
4. Consulta de exemplo
5. Link de documentação para a consulta de exemplo

:::image type="content" source="./images/getting-started.png" alt-text="Captura de tela da interface de usuário do Graph Explorer" border="true":::.

## <a name="make-a-get-request-in-graph-explorer"></a>Fazer uma solicitação GET no Graph Explorer

Para executar uma solicitação GET no Graph Explorer, você não precisa estar conectado. Basta escolher uma consulta de amostra e os dados de amostra são exibidos na visualização da resposta. 

:::image type="content" source="./images/making-a-get-request.png" alt-text="Captura de tela de uma solicitação de exemplo no Explorador do Graph." border="true":::

Para fazer uma solicitação:

1. Selecione uma consulta de exemplo e execute-a.
2. Obtenha o código de resposta HTTP.
3. Exiba a resposta da API do Microsoft Graph com dados de exemplo.

Quando você entra no Graph Explorer e escolhe a mesma consulta, a resposta é retornada com dados reais do locatário em que você entrou.

## <a name="run-non-get-requests-in-graph-explorer"></a>Executar solicitações não GET no Graph Explorer

Para tentar solicitações POST, PUT, PATCH e DELETE, entre no Graph Explorer usando uma conta do Microsoft 365. Pode ser uma conta organizacional para fins de teste ou demonstração. Para obter uma amostra grátis de assinatura de desenvolvedor do Microsoft 365 E5, junto com ferramentas e outros recursos para ajudá-lo a criar soluções para a plataforma Microsoft 365, associe-se ao [Programa de Desenvolvedor do Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program). 

>[!IMPORTANT]
>Se você optar por entrar usando sua conta organizacional, a execução de uma solicitação não GET poderá afetar os dados no locatário.

Por exemplo, para executar uma solicitação POST, selecione POST na lista suspensa para o verbo HTTP e adicione um corpo de solicitação e cabeçalhos de solicitação conforme apropriado.

:::image type="content" source="./images/making-a-post-request.png" alt-text="Captura de tela de uma solicitação POST no Explorador do Graph." border="true":::

1. Selecione uma consulta de exemplo POST.
2. Atualizar **Corpo da solicitação;** por exemplo, dê um nome ao aplicativo.
3. Selecione **Executar consulta**.
4. Consulte a resposta da API do Microsoft Graph.

Para visualizar a resposta em um formato diferente do JSON padrão, escolha a guia **Cabeçalhos de solicitação** no painel de solicitação, defina o par de chave/valor e selecione **Adicionar**.

:::image type="content" source="./images/adding-key-value-pairs.png" alt-text="Captura de tela que mostra a guia de Cabeçalhos de solicitação no Explorador do Graph." border="true":::

## <a name="next-steps"></a>Próximas etapas

- Experimente o [Explorador de Gráficos](https://developer.microsoft.com/graph/graph-explorer/).
- Saiba mais sobre o [Explorador do Graph](./graph-explorer-features.md).
- Contribua ou forneça comentários no [repositório do GitHub](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).
