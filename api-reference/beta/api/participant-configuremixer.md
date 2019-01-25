---
title: 'participante: configureMixer'
description: Configure como áudio misto para diferentes participantes em uma conversa com vários participantes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0be23ec4c9e7835c919328655e89880003546472
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530038"
---
# <a name="participant-configuremixer"></a>participante: configureMixer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configure como áudio misto para diferentes participantes em uma conversa com vários participantes.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
| :-------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Não suportado        |
| Delegado (conta pessoal da Microsoft) | Não suportado        |
| Aplicativo     | Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro      | Tipo    |Descrição|
|:---------------|:--------|:----------|
|participantMixerLevels|coleção [participantMixerLevel](../resources/participantmixerlevel.md)| Configuração do mixer redistribui para determinados participante de áudio.|
|ClientContext|String|O contexto de cliente.|

## <a name="response"></a>Resposta
Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/configureMixer
Content-Type: application/json
Content-Length: 501

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "participantMixerLevels": [
    {
      "participant": "550fae72-d251-43ec-868c-373732c2704f",
      "exclusive": true,
      "ducking": {
        "rampActive": 50,
        "rampInactive": 50,
        "lowerLevel": 10,
        "upperLevel": 50
      },
      "sourceLevels": [
        {
          "participant": "632899f8-2ea1-4604-8413-27bd2892079f",
          "level": 50,
          "duckOthers": false
        }
      ]
    }
  ]
}
```

##### <a name="response"></a>Resposta

> **Observação: **o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a>Notificação - operação concluída

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"1\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
