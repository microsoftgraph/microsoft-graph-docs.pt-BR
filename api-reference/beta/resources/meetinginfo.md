---
title: tipo de recurso meetingInfo
description: Informações de reunião especificadas para criar ou ingressar em uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ef9c2b86c9eb745ae6282a5d3cbce8a76dc31139
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006638"
---
# <a name="meetinginfo-resource-type"></a>tipo de recurso meetingInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esta é uma classe abstrata que contém informações específicas da reunião.
 
Para ingressar em uma reunião existente, você deve especificar o [organizerMeetingInfo](organizermeetinginfo.md) em combinação com o [chatInfo](./chatinfo.md)ou apenas o [tokenMeetingInfo](tokenmeetinginfo.md).


## <a name="derived-types"></a>Tipos derivados

| Tipo                                                 | Descrição                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [organizerMeetingInfo](./organizermeetinginfo.md)    | Detalhes sobre o organizador da reunião                          |
| [tokenMeetingInfo](tokenmeetinginfo.md)              | Um token criptografado que contém as informações sobre a reunião  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
