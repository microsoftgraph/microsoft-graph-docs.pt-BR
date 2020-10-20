---
title: tipo de recurso participantEndpoint
description: O tipo participantEndpoint
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0002659ac32eaa1c76ad6dfecefd2a1f59c070e9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601570"
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
