---
title: Usar o Explorador do Graph para experimentar as APIs do Microsoft Graph
description: Use o Explorador do Graph para experimentar as APIs do Microsoft Graph no locatário de exemplo padrão para explorar os recursos ou entre em seu próprio locatário e use-o como uma ferramenta de criação de protótipo para atender aos cenários do aplicativo.
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: 3f957d940d4dde483324492f1778ede970a5aefc
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013716"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a>Usar o Explorador do Graph para experimentar as APIs do Microsoft Graph

[O Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/) é uma ferramenta de desenvolvedor que permite que você faça convenientemente solicitações da API REST do Microsoft Graph e veja as respostas correspondentes. Use o Explorador do Graph para experimentar APIs no exemplo de locatário padrão para explorar as funcionalidades ou entre em seu próprio locatário e use-o como uma ferramenta de criação de protótipo para atender aos cenários do aplicativo. Essa ferramenta inclui recursos úteis, como trechos de código em C#, Java, JavaScript e Objective C; Integração de cartões adaptáveis e kits de ferramentas do Microsoft Graph; e muito mais.

Use o Explorador do Graph para:

- Faça solicitações da API do Microsoft Graph (GET, POST, PUT, PATCH e DELETE) e veja respostas, incluindo o código de resposta e quaisquer headers e corpos.
- Consentimento para permissões.
- Adicione um corpo de solicitação e um header de solicitação à sua consulta.
- Exibir e copiar o token de acesso.
- Veja exemplos de consultas para diferentes serviços no Microsoft Graph.
- Exibir, baixar ou excluir as consultas que você fez nos últimos 30 dias.
- Exibir e copiar trechos de código de cada consulta que você executar em C#, Java, JavaScript e Objective C.
- Acesse os componentes e cartões adaptáveis do Microsoft Graph Toolkit para algumas consultas de exemplo.
- Compartilhe consultas, incluindo o corpo da solicitação e os headers de solicitação.

O Explorador do Graph lida com o processo de autenticação para você. Personalize a experiência repondo a barra lateral e alterando o tema.

## <a name="get-started"></a>Introdução

O Graph Explorer é um aplicativo Web hospedado na central de desenvolvedores [do Microsoft Graph.](https://developer.microsoft.com/en-us/graph/graph-explorer) É um projeto de código aberto e damos as boas-vindas às suas contribuições e comentários no [repositório do GitHub.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4)

O Graph Explorer inclui os seguintes elementos:

1. Lista drop-down de verbo HTTP
2. Lista drop-down de versão da API
3. Barra de endereços de consulta de solicitação
4. Consulta de exemplo
5. Link de documentação para a consulta de exemplo

![Captura de tela da interface do usuário do Graph Explorer](./images/getting-started.png)

### <a name="make-a-get-request-in-graph-explorer"></a>Fazer uma solicitação GET no Explorador do Graph

Para executar uma solicitação GET no Explorador do Graph, você não precisa entrar. Basta clicar em um exemplo de consulta e mostrar dados de exemplo na visualização da resposta. 

![Captura de tela de uma solicitação de exemplo no Explorador do Graph](./images/making-a-get-request.png)

Para fazer uma solicitação:

1. Selecione uma consulta de exemplo e execute-a.
2. Obter o código de resposta HTTP.
3. Veja a resposta da API do Microsoft Graph com dados de exemplo.

Quando você entrar no Explorador do Graph e clicar na mesma consulta, a resposta será retornada com dados reais do locatário em que você se inscreveu.

### <a name="running-non-get-requests-in-graph-explorer"></a>Executando solicitações não GET no Explorador do Graph

Para experimentar solicitações POST, PUT, PATCH e DELETE, entre no Explorador do Graph usando uma conta do Microsoft 365. Pode ser uma conta organizacional para fins de teste ou demonstração. Para obter um exemplo gratuito de assinatura de desenvolvedor do Microsoft 365 E5, juntamente com ferramentas e outros recursos para ajudá-lo a criar soluções para a plataforma Microsoft 365, participe do Programa para Desenvolvedores [do Microsoft 365.](https://developer.microsoft.com/microsoft-365/dev-program) 

>[!IMPORTANT]
>Se você optar por entrar usando sua conta organizacional, executar uma solicitação não GET pode afetar os dados no locatário.

Por exemplo, para executar uma solicitação POST, selecione POST na lista drop-down para o verbo HTTP e adicione um corpo de solicitação e cabeçalhos de solicitação conforme apropriado.

![Captura de tela de uma solicitação POST no Explorador do Graph](./images/making-a-post-request.png)

1. Selecione uma consulta de exemplo POST.
2. Atualizar **corpo da solicitação;** por exemplo, dê um nome ao aplicativo.
3. Clique **em Executar consulta**.
4. Veja a resposta da API do Microsoft Graph.

Para exibir a resposta em um formato diferente do JSON padrão, escolha a guia Solicitação de **headers** no painel de solicitação, defina o par chave/valor e clique em **Adicionar**.

![Screenshot that shows the Request headers tab in Graph Explorer](./images/adding-key-value-pairs.png)

## <a name="next-steps"></a>Próximas etapas

- Visite [o Explorador do Graph.](https://developer.microsoft.com/graph/graph-explorer/)
- Saiba mais sobre os [recursos do Graph Explorer.](./graph-explorer-features.md)
- Contribuir ou fornecer comentários no [repositório do GitHub.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)
