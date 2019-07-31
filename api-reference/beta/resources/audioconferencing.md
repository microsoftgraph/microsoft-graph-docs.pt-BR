---
title: tipo de recurso audioConferencing
description: Representa as informações de acesso de telefone de um onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 94dc02920e7270fbfdacb10ee9a8edee8315fc67
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974280"
---
# <a name="audioconferencing-resource-type"></a>tipo de recurso audioConferencing

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de acesso de telefone de um [onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | String  | Uma URL para a página da Web acessível externamente que contém informações de discagem. |
| leaderPasscode      | String  | A senha de preenchimento necessária para se conectar ao provedor de conferência de áudio.      |
| participantPasscode | String  | A senha do participante necessária para se conectar ao provedor de conferência de áudio. |
| tollFreeNumber      | String  | O número de chamada gratuita para se conectar ao provedor de conferência de áudio.              |
| tollNumber          | String  | O número de chamada tarifada para se conectar ao provedor de conferência de áudio.                   |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
