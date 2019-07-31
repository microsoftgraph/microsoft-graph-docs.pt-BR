---
title: tipo de recurso synchronizationJobRestartCriteria
description: 'Define o escopo da ação [synchronizationJob: reiniciar](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8fb363b74f1daff678d0751aca4a9033b01d9832
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964652"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>tipo de recurso synchronizationJobRestartCriteria

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o escopo da ação [synchronizationJob: reiniciar](../api/synchronization-synchronizationjob-restart.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|resetScope|String| Combinação separada por vírgula dos seguintes `Full`valores:, `QuarantineState`, `Watermark`, `Escrows`,. `ConnectorDataStore` Use `Full` se você quiser todas as opções.|

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
  "resetScope": "String"
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
