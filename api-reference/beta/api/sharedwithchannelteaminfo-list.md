---
title: Listar sharedWithChannelTeamInfo
description: Obtenha a lista de equipes compartilhadas com um canal.
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: e57444da50bd0fbbd844b71e4a4ed6c5c914d3a4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212764"
---
# <a name="list-sharedwithchannelteaminfo"></a>Listar sharedWithChannelTeamInfo
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a lista de[equipes](../resources/sharedwithchannelteaminfo.md) com a qual foi compartilhado um [canal](../resources/channel.md) especificado. Esta operação é permitida somente para canais com valor **membershipType** de `shared`.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|ChannelMember.Read.All, ChannelMember.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|ChannelMember.Read.All, ChannelMember.ReadWrite.All |

> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/channels/{channel-id}/sharedWithTeams
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método oferece suporte aos parâmetros de consulta `$filter` e `$select`[OData](/graph/query-parameters)para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_sharedwithchannelteaminfo"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/sharedWithTeams
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sharedwithchannelteaminfo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sharedwithchannelteaminfo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sharedwithchannelteaminfo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sharedwithchannelteaminfo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-sharedwithchannelteaminfo-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-sharedwithchannelteaminfo-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.sharedWithChannelTeamInfo",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
      "id": "2173de69-de69-2173-69de-732169de7321",
      "tenantId": "b3246f44-b4gb-4627-96c6-25b18fa2c910",
      "displayName": "Team Contosso",
      "isHostTeam": true
    },
    {
      "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
      "id": "893075dd-2487-4122-86db-022c42e20265",
      "displayName": "Team fabricam",
      "isHostTeam": false,
      "tenantId": "b3246f44-b4gb-5678-96c6-25b18fa2c910"
    }
  ]
}
```

