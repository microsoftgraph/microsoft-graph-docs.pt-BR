---
title: tipo de recurso participante
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4a138267529127562fa9df42d8b20a985939b50e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345006"
---
# <a name="participant-resource-type"></a>tipo de recurso participante

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de participante.

## <a name="methods"></a>Métodos

| Método                                                          | Tipo de retorno                              | Descrição                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [Obter participante](../api/participant-get.md)                    | [participante](participant.md)            | Leia as propriedades do objeto **participante** .    |
| [ConfigureMixer](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | Configure o mixer de áudio do participante.            |
| [Convidar](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | Convidar um participante para a chamada.                 |
| [Ativar mudo para participante](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | Tirar o áudio de um participante em uma chamada.                     |
| [Ativar mudo de todos os participantes](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | Ativar mudo de todos os participantes da reunião.         |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                     | Descrição                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | A ID do participante.                                          |
| informações                  | [participantInfo](participantinfo.md)    | O participante do participante.                          |
| isInLobby            | booliano                                  | true se o participante está no lobby                          |
| IsMuted              | booliano                                  | true se o participante estiver mudo (cliente ou servidor sem som)    |
| mediaStreams         | coleção [mediaStream](mediastream.md) | A lista de fluxos de mídia.                                   |
| los             | String                                   | Um blob de dados fornecido pelo participante na lista     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Informações sobre o fato de o participante ter capacidade de gravação. |

## <a name="relationships"></a>Relações
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
  "suppressions": []
}
-->
