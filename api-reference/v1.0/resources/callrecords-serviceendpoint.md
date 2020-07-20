---
title: tipo de recurso serviceEndpoint
description: O tipo de serviceEndpoint
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f9120e1b35974a6e921eb269d289dfc82ba9e532
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491942"
---
# <a name="serviceendpoint-resource-type"></a>tipo de recurso serviceEndpoint

Namespace: microsoft.graph.callRecords

Representa um ponto de extremidade de serviço em uma chamada. O ponto de extremidade representa um servidor de mídia de chamada ou outra entidade de serviço. Herda de tipo de [ponto de extremidade](callrecords-endpoint.md) .

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
  "@odata.type": "microsoft.graph.callRecords.serviceEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
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
  "description": "serviceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->