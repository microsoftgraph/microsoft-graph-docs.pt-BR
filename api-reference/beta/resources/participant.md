---
title: tipo de recurso de participantes
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508143"
---
# <a name="participant-resource-type"></a>tipo de recurso de participantes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de participante.

## <a name="methods"></a>Métodos

| Método                                                          | Tipo de retorno                              | Descrição                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [Obtenha um participante](../api/participant-get.md)                    | [participante](participant.md)            | Leia as propriedades do objeto **participante** .    |
| [ConfigureMixer](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | Configure o participante mixer de áudio.            |
| [Convidar](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | Convide um participante à chamada.                 |
| [Ativar Mudo participante](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | Ativar Mudo de um participante em uma chamada.                     |
| [Ativar Mudo de todos os participantes](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | Ativar Mudo de todos os participantes da reunião.         |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                     | Descrição                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | A identificação dos participantes.                                          |
| Info                 | [participantInfo](participantinfo.md)    | O participante do participante.                          |
| isInLobby            | booliano                                  | True se o participante estiver no lobby                          |
| isMuted              | booliano                                  | True se o participante está sem som (cliente ou servidor sem áudio)    |
| mediaStreams         | coleção [mediaStream](mediastream.md) | A lista de fluxos de mídia.                                   |
| Metadata             | String                                   | Um blob de dados fornecidos pelo participante na lista     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Informações sobre se o participante tenha o recurso de gravação. |

## <a name="relationships"></a>Relacionamento
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
}
```

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
