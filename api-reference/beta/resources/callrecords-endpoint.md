---
title: tipo de recurso de ponto de extremidade
description: O tipo de ponto de extremidade
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f17aa21de65fef33b0c7e4a94151eab4f49583ac
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394673"
---
# <a name="endpoint-resource-type"></a>tipo de recurso de ponto de extremidade

Namespace: Microsoft. Graph. callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um ponto de extremidade em uma chamada. O ponto de extremidade pode ser o dispositivo de um usuário, uma reunião, um aplicativo/bot, etc. Os tipos [participantEndpoint](callrecords-participantendpoint.md) e [serviceEndpoint](callrecords-serviceendpoint.md) herdam desse tipo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|userAgent|[Microsoft. Graph. callRecords. UserAgent](callrecords-useragent.md)|Agente de usuário relatado por este ponto de extremidade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.endpoint",
  "baseType": null
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->