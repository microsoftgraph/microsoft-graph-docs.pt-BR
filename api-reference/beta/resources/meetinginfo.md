---
title: Tipo de recurso meetingInfo
description: Informações de reunião especificadas para criar ou ingressar em uma reunião.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d7aebdbd0236f0c1223e295456d408f37fb0708e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731586"
---
# <a name="meetinginfo-resource-type"></a>Tipo de recurso meetingInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Essa é uma classe abstrata que contém informações específicas da reunião.
 
Para ingressar em uma reunião existente, você deve especificar o [organizerMeetingInfo](organizermeetinginfo.md) em combinação com [o chatInfo](./chatinfo.md), [o tokenMeetingInfo](tokenmeetinginfo.md) ou [o joinMeetingIdMeetingInfo](joinmeetingidmeetinginfo.md).


## <a name="derived-types"></a>Tipos derivados

| Tipo                                                    | Descrição                                                         |
|:--------------------------------------------------------|:--------------------------------------------------------------------|
| [joinMeetingIdMeetingInfo](joinmeetingidmeetinginfo.md) | Contém **o joinMeetingId** **e a senha** da reunião.     |
| [organizerMeetingInfo](./organizermeetinginfo.md)       | Detalhes sobre o organizador da reunião.                         |
| [tokenMeetingInfo](tokenmeetinginfo.md)                 | Um token criptografado que contém as informações sobre a reunião. |

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


