---
title: tipo de recurso de ponto de extremidade
description: O tipo de ponto de extremidade
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4fe19bd5a69b456a0e74e70b118477131f7c8f2cb0011eac4270dad956d6667c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252120"
---
# <a name="endpoint-resource-type"></a>tipo de recurso de ponto de extremidade

Namespace: microsoft.graph.callRecords

Representa um ponto de extremidade em uma chamada. O ponto de extremidade pode ser um dispositivo do usuário, uma reunião, um aplicativo/bot, etc. Os [tipos participantEndpoint](callrecords-participantendpoint.md) [e serviceEndpoint](callrecords-serviceendpoint.md) herdam desse tipo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|userAgent|[microsoft.graph.callRecords.userAgent](callrecords-useragent.md)|Agente de usuário relatado por esse ponto de extremidade.|

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
