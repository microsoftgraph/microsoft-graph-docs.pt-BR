---
title: Tipo de recurso participantEndpoint
description: O tipo participantEndpoint
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d83690c1209d845f00dc902170eb547c567d6ec0cc654d6c9e9c3778da0fc275
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223729"
---
# <a name="participantendpoint-resource-type"></a>Tipo de recurso participantEndpoint

Namespace: microsoft.graph.callRecords

Representa um ponto de extremidade do participante em uma chamada. O ponto de extremidade representa um usuário ou entidade do tipo usuário. Herda do [tipo de ponto de](callrecords-endpoint.md) extremidade.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|userAgent|[microsoft.graph.callRecords.userAgent](callrecords-useragent.md)|Agente de usuário relatado por esse ponto de extremidade.|
|comentários|[microsoft.graph.callRecords.userFeedback](callrecords-userfeedback.md)|Os comentários fornecidos pelo usuário deste ponto de extremidade sobre a qualidade da sessão.|
|identity|[identitySet](identityset.md)|Identidade associada ao ponto de extremidade.|

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
