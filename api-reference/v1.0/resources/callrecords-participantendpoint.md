---
title: tipo de recurso participantEndpoint
description: O tipo participantEndpoint
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ff590acb76d50da9d0772bdaece805a1db0cd26a
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491966"
---
# <a name="participantendpoint-resource-type"></a>tipo de recurso participantEndpoint

Namespace: microsoft.graph.callRecords

Representa um ponto de extremidade de participante em uma chamada. O ponto de extremidade representa uma entidade de usuário ou semelhante a um usuário. Herda de tipo de [ponto de extremidade](callrecords-endpoint.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|userAgent|[Microsoft. Graph. callRecords. UserAgent](callrecords-useragent.md)|Agente de usuário relatado por este ponto de extremidade.|
|comentários|[Microsoft. Graph. callRecords. userfeedback](callrecords-userfeedback.md)|Os comentários fornecidos pelo usuário deste ponto de extremidade sobre a qualidade da sessão.|
|ladrões|[identitySet](identityset.md)|Identidade associada ao ponto de extremidade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.participantEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"},
  "feedback": {"@odata.type": "microsoft.graph.callRecords.userFeedback"},
  "identity": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->