---
title: tipo de recurso securityResource
description: Representa os recursos relacionados a um alerta.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ce0398ba134f7537420a99ccaed84f2ff209f883
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682016"
---
# <a name="securityresource-resource-type"></a>tipo de recurso securityResource

Namespace: microsoft.graph

Representa os recursos relacionados a um alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|recurso|String|Nome do recurso relacionado ao alerta atual. **Obrigatório**.|
|resourceType|[securityResourceType](#securityresourcetype-values)|Representa o tipo de recursos de segurança relacionados a um alerta. Os valores possíveis são: `attacked` e `related`.|

### <a name="securityresourcetype-values"></a>valores de securityResourceType

|Membro|Valor|Descrição|
|-|-|-|
|atacada|1 |O recurso foi atacado no alerta.|
|correspondente|duas|O recurso está relacionado ao alerta, embora não seja atacado diretamente.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.securityResource"
}-->

```json
{
  "resource": "String",
  "resourceType": "@odata.type: microsoft.graph.securityResourceType"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
