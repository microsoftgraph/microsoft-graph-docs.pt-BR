---
title: Usar Graph Explorer para experimentar APIs do Microsoft Graph
description: Use o Graph Explorer para tentar apIs do Microsoft Graph no locatário de exemplo padrão para explorar recursos ou entrar no seu próprio locatário e usá-lo como uma ferramenta de prototipagem para atender aos cenários do aplicativo.
ms.localizationpriority: medium
author: bettirosengugi
ms.openlocfilehash: 10929ab2a8dfccc54ccf7cab93e0274716b4aad8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59014318"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a>Usar Graph Explorer para experimentar APIs do Microsoft Graph

[Graph Explorer é](https://developer.microsoft.com/graph/graph-explorer/) uma ferramenta de desenvolvedor que permite que você faça convenientemente solicitações de API REST da Microsoft Graph exibir respostas correspondentes. Use Graph Explorer para experimentar APIs no locatário de exemplo padrão para explorar recursos ou entrar no seu próprio locatário e usá-lo como uma ferramenta de prototipagem para atender aos cenários do aplicativo. Esta ferramenta inclui recursos úteis, como trechos de código em C#, Java, JavaScript e Objective C; Integração Graph Toolkit cartões adaptáveis e da Microsoft; e muito mais.

Use Graph Explorer para:

- Faça solicitações Graph API da Microsoft (GET, POST, PUT, PATCH e DELETE) e consulte respostas, incluindo código de resposta e quaisquer headers e corpos.
- Consentimento para permissões.
- Adicione um corpo de solicitação e um header de solicitação à consulta.
- Exibir e copiar o token de acesso.
- Exibir consultas de exemplo para diferentes serviços no Microsoft Graph.
- Exibir, baixar ou excluir as consultas que você fez nos últimos 30 dias.
- Exibir e copiar trechos de código de cada consulta que você executar em C#, Java, JavaScript e Objetivo C.
- Acesse os Graph Toolkit microsoft e cartões adaptáveis para algumas consultas de exemplo.
- Compartilhe consultas, incluindo o corpo da solicitação e os headers de solicitação.

Graph O Explorer lida com o processo de autenticação para você. Personalize a experiência desmontando a barra lateral e alterando o tema.

## <a name="get-started"></a>Introdução

Graph O Explorer é um aplicativo Web hospedado no centro de desenvolvedores [do Microsoft Graph.](https://developer.microsoft.com/en-us/graph/graph-explorer) É um projeto de código aberto e saudamos suas contribuições e comentários no [GitHub repo.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4)

Graph O Explorer inclui os seguintes elementos:

1. Lista drop-down do verbo HTTP
2. Lista de versões da API lista listada
3. Barra de endereços de consulta de solicitação
4. Consulta de exemplo
5. Link de documentação para a consulta de exemplo

![Captura de tela da interface do usuário Graph Explorer](./images/getting-started.png)

### <a name="make-a-get-request-in-graph-explorer"></a>Fazer uma solicitação GET no Graph Explorer

Para executar uma solicitação GET no Graph Explorer, não é preciso entrar. Basta clicar em uma consulta de exemplo e os dados de exemplo mostrarão na visualização da resposta. 

![Captura de tela de uma solicitação de exemplo no Graph Explorer](./images/making-a-get-request.png)

Para fazer uma solicitação:

1. Selecione uma consulta de exemplo e execute-a.
2. Obter o código de resposta HTTP.
3. Consulte a resposta da API do Microsoft Graph com dados de exemplo.

Quando você entrar no Graph Explorer e clicar na mesma consulta, a resposta será retornada com dados reais do locatário em que você se inscreveu.

### <a name="running-non-get-requests-in-graph-explorer"></a>Executando solicitações não GET no Graph Explorer

Para experimentar solicitações POST, PUT, PATCH e DELETE, entre no Graph Explorer usando uma conta Microsoft 365. Pode ser uma conta organizacional para fins de teste ou demonstração. Para obter uma assinatura gratuita de Microsoft 365 E5 desenvolvedor, juntamente com ferramentas e outros recursos para ajudá-lo a criar soluções para a plataforma Microsoft 365, participe do programa Microsoft 365 [Desenvolvedor.](https://developer.microsoft.com/microsoft-365/dev-program) 

>[!IMPORTANT]
>Se você optar por entrar usando sua conta organizacional, executar uma solicitação não GET poderá afetar os dados no locatário.

Por exemplo, para executar uma solicitação POST, selecione POST na lista drop-down do verbo HTTP e adicione um corpo de solicitação e cabeçalhos de solicitação conforme apropriado.

![Captura de tela de uma solicitação POST no Graph Explorer](./images/making-a-post-request.png)

1. Selecione uma consulta de exemplo POST.
2. Atualizar **corpo da solicitação;** por exemplo, dê um nome ao aplicativo.
3. Clique **em Executar consulta**.
4. Consulte a resposta da API Graph Microsoft.

Para exibir a resposta em um formato diferente do JSON padrão, escolha a guia Solicitar **headers** no painel de solicitação, defina o par chave/valor e clique em **Adicionar**.

![Captura de tela que mostra a guia Solicitação de headers no Graph Explorer](./images/adding-key-value-pairs.png)

## <a name="next-steps"></a>Próximas etapas

- Visite [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/).
- Saiba mais sobre Graph [recursos do Explorer.](./graph-explorer-features.md)
- Contribuir ou fornecer comentários no [GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).
