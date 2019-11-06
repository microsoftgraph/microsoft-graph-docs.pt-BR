---
title: tipo de recurso participante
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e2fae206fb76ffe3c00b91d992c874e200eeae98
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006596"
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
| [Participante sem áudio](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | Tirar o áudio de um participante em uma chamada.                     |
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
