---
title: tipo de recurso audioConferencing
description: Representa as informações de acesso de telefone de um onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1371e80830bf148588f6bda91326b0521fcdda42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328364"
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
