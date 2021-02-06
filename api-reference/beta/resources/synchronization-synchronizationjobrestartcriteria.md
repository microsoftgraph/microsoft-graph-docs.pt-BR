---
title: Tipo de recurso synchronizationJobRestartCriteria
description: 'Define o escopo da ação synchronizationJob: restart.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ef15c9322c553d0eedb977c3f01ed5de2823e844
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136497"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>Tipo de recurso synchronizationJobRestartCriteria

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o escopo da ação [synchronizationJob: restart.](../api/synchronization-synchronizationjob-restart.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|resetScope|String| Combinação separada por vírgulas dos seguintes valores: `Full` , `QuarantineState` , , `Watermark` `Escrows` `ConnectorDataStore` . Use `Full` se quiser todas as opções.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
    "criteria": {
        "resetScope": "String"
    }
}


```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


