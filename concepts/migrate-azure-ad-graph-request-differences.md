---
title: Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph
description: Descreve como as solicitações do Microsoft Graph são diferentes das solicitações do Azure AD, o que ajuda a migrar aplicativos para o serviço mais recente..
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f046043b6a30d66cef96bb6eb6192bddd90d2f5f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630206"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a>Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1:* revisar as diferenças de API do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

O Microsoft Graph e a API do Azure AD Graph são APIs REST e cada uma suportam convenções ODATA para parâmetros de consulta. No entanto, a sintaxe varia entre essas duas APIs.

Use o [Explorador do Graph](https://aka.ms/ge) para experimentar esses padrões de solicitação em seus próprios dados, pois é uma ótima maneira de aprender sobre as diferenças de solicitação e resposta.

## <a name="basic-requests"></a>Solicitações básicas

A tabela a seguir realça as principais diferenças de solicitação entre as duas APIs:

|| Gráfico do Azure AD | Microsoft Graph |
|---|---|---|
|Sintaxe de solicitação| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|Pontos&nbsp;de extremidade de serviço:||
|-&nbsp;Global|`https://graph.windows.net`|`https://graph.microsoft.com`|
|-&nbsp;L4&nbsp;gov&nbsp;(EUA)|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|-&nbsp;(DoD) de US gov&nbsp;&nbsp;&nbsp;|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|-&nbsp;Alemanha|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|-&nbsp;China&nbsp;(21vianet)| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|{tenant_id}|Especifique a ID do locatário na solicitação.|É opcional especificar uma ID de locatário na solicitação, pois ela é inferida do token de acesso.<br><br>Se você especificar a ID do locatário, ela vai entre `{version}` o e `{resource}` o na URL da solicitação.|
|Version|Especifique a versão de lançamento do Graph do Azure AD na solicitação usando um parâmetro de consulta necessário.|Especifique a versão de lançamento do Microsoft Graph na solicitação como parte do caminho da URL imediatamente após o ponto de extremidade do serviço.|

Você pode continuar a usar os mesmos parâmetros de consulta no Microsoft Graph como o Graph do Azure AD.

### <a name="example-request-comparison"></a>Exemplo de comparação de solicitação

Suponha que você queira uma lista de todos os usuários com nomes que começam com "Dan".

No Azure AD Graph, você pode usar essa solicitação:

`https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6`

Esta solicitação:

- Targets versão 1,6 do Azure AD Graph.  
- Especifica `contoso.com` como a ID do locatário.  
- Chama o recurso users.  
- Usa o `$filter` parâmetro de consulta para limitar a resposta a determinados nomes que começam `Dan`com.  

Os resultados incluem usuários com nomes como Daniel, Danforth, Danielle, DANERYS e assim por diante.

Uma solicitação semelhante para o Microsoft Graph seria:

`https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

Nela

- A versão é `v1.0`.  
- A ID do locatário é inferida do token de acesso (não mostrado).  
- O parâmetro de `$filter` recurso e de consulta é o mesmo que a consulta do Azure AD.  

> **Observação**: se você estiver usando a biblioteca de cliente .net do Azure ad Graph, confira [bibliotecas de clientes .net](migrate-azure-ad-graph-client-libraries.md) para obter estratégias e assistência mais específicas para mover para a biblioteca de cliente .net do Microsoft Graph.

### <a name="key-identifiers-objectid-vs-id"></a>Identificadores de chave: objectId vs ID

No gráfico do Azure AD, todos os tipos de recursos de entidade têm um identificador (ou chave) exclusivo chamado **ObjectID**.  Para a maior parte (salvo indicação em contrário) esse mesmo identificador é chamado de **ID** no Microsoft Graph.

## <a name="default-properties-and-select"></a>Propriedades e $select padrão

Use o `$select` parâmetro de consulta, em solicitações GET, para personalizar a resposta para incluir todas as propriedades exigidas pelo seu aplicativo.

As operações de **obtenção** ou **lista** do Microsoft Graph para recursos de usuário ou grupo retornam apenas um subconjunto de todas as propriedades, conhecidas como _propriedades padrão_. As propriedades padrão representam as propriedades mais comumente usadas para um recurso. Por outro lado, o Azure AD Graph retorna o conjunto completo de todas as propriedades do respectivo recurso.

Para obter outras propriedades na v 1.0, seu aplicativo precisa solicitá-las explicitamente, usando `$select` o parâmetro de consulta. Isso inclui todas as extensões de esquema de diretório que o aplicativo pode estar usando. É uma prática recomendada solicitar apenas as propriedades que seu aplicativo realmente precisa.

Para ilustrar a diferença, use o explorador do Graph para executar as seguintes solicitações e comparar as diferentes respostas.

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

Revise as respostas de cada consulta. Você notará que as informações de endereço são retornadas pela versão/beta, mas não pela versão/v1.0.  Isso ocorre porque as propriedades address não estão no conjunto de propriedades padrão.

Se seu aplicativo depende das propriedades de endereço, você precisa atualizar suas solicitações v 1.0 para incluir o parâmetro de `$select` consulta:

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

A resposta para esta solicitação incluiria as propriedades de endereço.  Ele também inclui a propriedade **DisplayName** , mas somente porque foi especificado pelo parâmetro de consulta.

Saiba mais sobre:

- Propriedades padrão no usuário, consulte [usuários](/graph/api/resources/users?view=graph-rest-1.0)
- O `$select` parâmetro e outros parâmetros de consulta ODATA suportados, confira [usar parâmetros de consulta para personalizar respostas](/graph/query-parameters).
- Esta e outras otimizações recomendadas, consulte [práticas recomendadas](/graph/best-practices-concept).

## <a name="relationships-and-navigation-properties"></a>Propriedades de relações e navegação

Relações (ou propriedades de navegação) são um conceito importante no gráfico do Azure AD e no Microsoft Graph, criando uma rede de recursos relacionados. Por exemplo, as propriedades **Manager** e **DirectReports** estendem o recurso User para fornecer a hierarquia organizacional.  

As relações também definem associações, como os grupos aos quais um usuário pertence, os membros que pertencem a um grupo ou uma função de diretório e assim por diante.

As solicitações do Azure AD `$link` Graph usam para indicar relações entre recursos.  No Microsoft Graph, isso usa a notação ODATA 4, 1 `$ref` em vez disso.

A tabela a seguir mostra vários exemplos:

| Tarefa | Gráfico do Azure AD | Microsoft Graph |
|------|----------------|-----------------|
| Adicionar membro        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| Listar links de membros | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| Listar membros      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| Remover membro     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

Ao migrar seus aplicativos para o Microsoft Graph, procure solicitações que `$link` usam para associar recursos; Altere-os para `$ref` usar em seu lugar.

## <a name="next-steps"></a>Próximos passos

- Saiba mais sobre as [diferenças de recursos de serviço](migrate-azure-ad-graph-feature-differences.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
