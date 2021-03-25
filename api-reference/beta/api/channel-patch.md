---
title: 'Canal de Atualização '
description: Atualize as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f20b72ef2840b5fcaa45985ee83f544df250d92f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200928"
---
# <a name="update-channel"></a>Canal de Atualização 

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do canal [especificado](../resources/channel.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | ChannelSettings.ReadWrite.Group*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}/channels/{channel-id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).

> **Observação:** Não é possível atualizar `membershipType` o valor de um canal existente.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="example-1-update-channel"></a>Exemplo 1: canal de atualização

#### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```

#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-channel-with-moderation-settings"></a>Exemplo 2: Atualizar canal com configurações de moderação

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação para atualizar as [configurações de moderação](../resources/channelmoderationsettings.md) de um canal. Essa operação só pode ser executada por um proprietário da equipe.


<!-- {
  "blockType": "request",
  "name": "patch_channel_with_moderationSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
Content-type: application/json

{
    "displayName": "UpdateChannelModeration",
    "description": "Update channel moderation.",
    "moderationSettings": {
        "userNewMessageRestriction": "moderators",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```



#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


