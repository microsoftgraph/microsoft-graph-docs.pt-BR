---
title: Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph
description: Descreve como as solicitações Graph microsoft diferem das solicitações do Azure AD, o que ajuda a migrar aplicativos para o serviço mais novo..
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 7a127393a6f0daf7743384b95b30e7ed7a1a16ff97522c4cad3b7d2317599b0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129621"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a>Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

O Microsoft Graph e a API de Graph do Azure AD são APIs REST e cada uma delas oferece suporte a convenções ODATA para parâmetros de consulta. No entanto, a sintaxe varia entre essas duas APIs.

Use o [Graph Explorer](https://aka.ms/ge) para experimentar esses padrões de solicitação em relação aos seus próprios dados, pois é uma ótima maneira de aprender sobre as diferenças de solicitação e resposta.

## <a name="basic-requests"></a>Solicitações básicas

A tabela a seguir destaca as principais diferenças de solicitação entre as duas APIs:

|Solicitar detalhes| Azure AD Graph. | Microsoft Graph |
|---|---|---|
|Sintaxe de solicitação| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|Pontos &nbsp; de extremidade do serviço:||
|-&nbsp;Global|`https://graph.windows.net`|`https://graph.microsoft.com`|
|-&nbsp;US &nbsp; Gov &nbsp; L4|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|-&nbsp;US &nbsp; Gov &nbsp; L5 &nbsp; (DOD)|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|-&nbsp;Alemanha|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|-&nbsp;China &nbsp; (21Vianet)| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|{tenant_id}|Especifique a ID do locatário na solicitação.|É opcional especificar uma ID de locatário na solicitação, pois ela é inferida do token de acesso.<br><br>Se você especificar a ID do locatário, ela fica entre a URL e `{version}` `{resource}` a da solicitação.|
|{version}|Especifique a versão de versão do Azure AD Graph na solicitação usando um parâmetro de consulta necessário.|Especifique a versão de versão do Microsoft Graph na solicitação como parte do caminho da URL logo após o ponto de extremidade do serviço.|

Você pode continuar a usar os mesmos parâmetros de consulta no Microsoft Graph que o Azure AD Graph.

### <a name="example-request-comparison"></a>Comparação de solicitação de exemplo

Suponha que você queira uma lista de todos os usuários com nomes começando com "Dan".

No Azure AD Graph, você pode usar esta solicitação:

`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` ou

`GET https://graph.windows.net/myOrganization/users?$filter=startswith(givenName,'Dan')&api-version=1.6`


Esta solicitação:

- Direciona a versão 1.6 do Azure AD Graph.
- Especifica como `contoso.com` a ID do locatário. A alternativa mostra o uso de um alias com base na ID do `myOrganization` locatário no token de acesso.
- Chama o recurso users.
- Usa o `$filter` parâmetro de consulta para limitar a resposta a determinados nomes que começam com `Dan` .

Os resultados incluem usuários com nomes como Daniel, Danforth, Danielle, Danerys e assim por diante.

Uma solicitação semelhante para o Microsoft Graph seria:

`GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

Aqui:

- A versão é `v1.0` .
- A ID do locatário é inferida do token de acesso (não mostrado).
- O parâmetro resource and query é o mesmo que a consulta `$filter` do Azure AD.

> **OBSERVAÇÃO**: Se você estiver usando a biblioteca de clientes do Azure AD Graph .NET, consulte Bibliotecas de clientes [.NET](migrate-azure-ad-graph-client-libraries.md) para obter estratégias e assistência mais específicas para mover para a biblioteca de clientes do Microsoft Graph .NET.

### <a name="key-identifiers-objectid-vs-id"></a>Identificadores de chave: objectId vs id

No Azure AD Graph, todos os tipos de recursos de entidade têm um identificador exclusivo (ou chave) chamado **objectId**.  Na maior parte (a menos que seja declarado de outra forma), esse mesmo identificador é chamado **de id** no Microsoft Graph.

## <a name="default-properties-and-select"></a>Propriedades padrão e $select

Use o parâmetro de consulta, em solicitações GET, para personalizar a resposta para incluir todas as `$select` propriedades que seu aplicativo exige.

O Microsoft Graph **obter** ou **listar** operações para recursos de usuário ou grupo retorna apenas um subconjunto de todas as propriedades, conhecidas como _propriedades padrão_. As propriedades padrão representam as propriedades mais comumente usadas para um recurso. Por outro lado, o Azure AD Graph retorna o conjunto completo de todas as propriedades do respectivo recurso.

Para obter outras propriedades em v1.0, seu aplicativo precisa solicitá-las explicitamente, usando o `$select` parâmetro de consulta. Isso inclui qualquer extensão de esquema de diretório que seu aplicativo possa estar usando. É uma prática prática só solicitar as propriedades que seu aplicativo realmente precisa.

Para ilustrar a diferença, use Graph Explorer para executar as seguintes solicitações e comparar as diferentes respostas.

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

Revise as respostas de cada consulta. Você notará que as informações de endereço são retornadas pela versão /beta, mas não pela versão /v1.0.  Isso porque as propriedades de endereço não estão no conjunto de propriedades padrão.

Se o aplicativo se basear nas propriedades de endereço, você precisará atualizar suas solicitações v1.0 para incluir o `$select` parâmetro de consulta:

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

A resposta para essa solicitação incluiria as propriedades de endereço.  Ele também inclui a **propriedade displayName,** mas somente porque foi especificada pelo parâmetro de consulta.

Para saber mais sobre:

- Propriedades padrão no usuário, consulte [users](/graph/api/resources/users?view=graph-rest-1.0)
- O parâmetro e outros parâmetros de consulta ODATA com `$select` suporte, consulte [Use query parameters to customize responses](./query-parameters.md).
- Esta e outras otimizações recomendadas, consulte [Práticas recomendadas.](./best-practices-concept.md)

## <a name="relationships-and-navigation-properties"></a>Relações e propriedades de navegação

As relações (ou propriedades de navegação) são um conceito-chave no Azure AD Graph microsoft Graph, criando uma rede de recursos relacionados. Por exemplo, as **propriedades manager** e **directReports** estendem o recurso do usuário para fornecer hierarquia organizacional.

As relações também definem associações, como os grupos aos quais um usuário pertence, os membros pertencentes a um grupo ou a uma função de diretório e assim por diante.

As solicitações do Azure AD Graph `$link` para indicar relações entre recursos.  No Microsoft Graph isso usa a notação ODATA 4.01. `$ref`

A tabela a seguir mostra vários exemplos:

| Tarefa | Azure AD Graph. | Microsoft Graph |
|------|----------------|-----------------|
| Adicionar membro        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| Listar links de membros | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| Listar membros      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| Remover membro     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

Ao migrar seus aplicativos para o Microsoft Graph, procure solicitações que usem para associar `$link` recursos; altere-os para `$ref` usar.

## <a name="next-steps"></a>Próximos passos

- Saiba mais [sobre as diferenças de](migrate-azure-ad-graph-feature-differences.md) recursos de serviço entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.