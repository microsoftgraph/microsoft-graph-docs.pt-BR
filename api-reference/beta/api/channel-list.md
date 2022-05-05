---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: akjo
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: bafd98995981238929dd311092c3d3e3d72d8d75
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211915"
---
# <a name="list-channels"></a>Listar canais

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All **, Group.ReadWrite.All**, Directory.Read.All **, Directory.ReadWrite.All** |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All **, Group.ReadWrite.All**, Directory.Read.All **, Directory.ReadWrite.All** |

[!INCLUDE [teamwork-permissions-note](../../../includes/teamwork-permissions-note.md)]

> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

### <a name="use-select-for-better-performance"></a>Use $select para melhorar o desempenho
Preencher as propriedades **email** e **moderationSettings** de um canal é uma operação cara que resulta em desempenho lento. Use `$select` para excluir o **email** e as propriedades **moderationSettings** para melhorar o desempenho.


## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-all-channels"></a>Exemplo 1: Listar todos os canais

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação para listar todos os canais.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-channels-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-channels-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Esta é a resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
      "membershipType": "standard"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a>Exemplo 2: Listar todos os canais privados

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação para listar todos os canais privados.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-private-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-private-channels-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-private-channels-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "19:982abbfca323a582f0a6d00ae2deca@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "test private team",
      "membershipType": "private"
    }
  ]
}
```

### <a name="example-3-list-all-shared-channels"></a>Exemplo 3: listar todos os canais compartilhados

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação para listar todos os canais compartilhados.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_shared_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6a720ba5-7373-463b-bc9f-4cd04b5c6742/channels?$filter=membershipType eq 'shared'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-shared-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-shared-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-shared-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-shared-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-shared-channels-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('6a720ba5-7373-463b-bc9f-4cd04b5c6742')/channels",
    "@odata.count": 1,
    "value": [
        {
            "id": "19:LpxShHZZh9utjNcEmUS5aOEP9ASw85OUn05NcWYAhX81@thread.tacv2",
            "createdDateTime": null,
            "displayName": "shared channel-01",
            "description": "this is the shared channel description",
            "isFavoriteByDefault": null,
            "email": "",
            "webUrl": "https://teams.microsoft.com/l/channel/19%3ALpxShHZZh9utjNcEmUS5aOEP9ASw85OUn05NcWYAhX81%40thread.tacv2/shared%20channel-01?groupId=6a720ba5-7373-463b-bc9f-4cd04b5c6742&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607",
            "membershipType": "shared",
            "moderationSettings": null
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
