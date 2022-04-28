---
title: Obter sharedWithChannelTeamInfo
description: Obtenha uma equipe compartilhada com um canal.
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 35d6fb0aa5323df0494d3ec3ccd2a4ae11ee9ae4
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061136"
---
# <a name="get-sharedwithchannelteaminfo"></a>Obter sharedWithChannelTeamInfo
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma [equipe](../resources/sharedwithchannelteaminfo.md) que foi compartilhada em um [canal](../resources/channel.md) especificado. Esta operação é permitida somente para canais com valor **membershipType** de `shared`.

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
GET /teams/{team-id}/channels/{channel-id}/sharedWithTeams/{shared-with-channel-team-info-id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método não dá suporte aos parâmetros de consulta OData ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_sharedwithchannelteaminfo"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/sharedWithTeams/893075dd-2487-5634-925f-022c42e20265
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedWithChannelTeamInfo"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
    "id": "2173de69-de69-2173-69de-732169de7321",
    "tenantId": "b3246f44-b4gb-4627-96c6-25b18fa2c910",
    "displayName": "Team contosso",
    "isHostTeam": true
  }
}
```

