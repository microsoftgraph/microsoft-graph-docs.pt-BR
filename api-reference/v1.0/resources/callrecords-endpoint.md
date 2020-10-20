---
title: tipo de recurso de ponto de extremidade
description: O tipo de ponto de extremidade
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3caf85f049c0b09caf5ae2ec3866ce9d24b2a1e8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601472"
---
# <a name="endpoint-resource-type"></a>tipo de recurso de ponto de extremidade

Namespace: microsoft.graph.callRecords

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
