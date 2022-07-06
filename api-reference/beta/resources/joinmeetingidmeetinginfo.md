---
title: Tipo de recurso joinMeetingIdMeetingInfo
description: Contém informações que permitem que você ingresse em uma reunião existente com uma joinMeetingId e uma senha.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a35dff2db37686bae85a52d47a4b1f1aa3a10ff0
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645583"
---
# <a name="joinmeetingidmeetinginfo-resource-type"></a>Tipo de recurso joinMeetingIdMeetingInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações que permitem que você ingresse em uma reunião existente com **uma joinMeetingId** **e uma senha** (se necessário). Você pode recuperar essas propriedades da API [Get onlineMeeting](../api/onlinemeeting-get.md) .

Herda de [meetingInfo](../resources/meetinginfo.md).

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo    | Descrição                                                   |
| :---------------------- | :------ | :------------------------------------------------------------ |
| joinMeetingId           | Cadeia de Caracteres  | A ID usada para ingressar na reunião.                              |
| senha                | Cadeia de caracteres  | A senha usada para ingressar na reunião. Opcional.              |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.joinMeetingIdMeetingInfo"
}-->
```json
{
    "joinMeetingId": "String",
    "passcode": "String"
}
```
