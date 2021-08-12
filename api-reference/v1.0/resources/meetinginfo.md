---
title: Tipo de recurso meetingInfo
description: Informações de reunião especificadas para criar ou ingressar em uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab866ada9fa4b886cbd90cb999132ff13b48d74437f11710a43aee31ba7857fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126407"
---
# <a name="meetinginfo-resource-type"></a>Tipo de recurso meetingInfo

Namespace: microsoft.graph

Esta é uma classe abstrata que contém informações específicas da reunião.
 
Para ingressar em uma reunião existente, você deve especificar o [organizerMeetingInfo](organizermeetinginfo.md) em combinação com [o chatInfo](./chatinfo.md)ou apenas [o tokenMeetingInfo](tokenmeetinginfo.md).


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

