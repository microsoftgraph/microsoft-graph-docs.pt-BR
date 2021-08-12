---
title: Tipo de recurso serviceEndpoint
description: O tipo serviceEndpoint
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dc51a13e8c244c8c4564dab9cf18dc5b28a450947c0ced8889aea8d6511d39a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216942"
---
# <a name="serviceendpoint-resource-type"></a>Tipo de recurso serviceEndpoint

Namespace: microsoft.graph.callRecords

Representa um ponto de extremidade de serviço em uma chamada. O ponto de extremidade representa um servidor de mídia de chamada ou outra entidade de serviço. Herda do [tipo de ponto de](callrecords-endpoint.md) extremidade.

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
