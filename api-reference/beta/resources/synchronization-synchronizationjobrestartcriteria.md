---
title: tipo de recurso synchronizationJobRestartCriteria
description: 'Define o escopo da ação [synchronizationJob: reiniciar](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c8992104493e7f59b1ddc74c7128dda50b2bfd9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520062"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>tipo de recurso synchronizationJobRestartCriteria

Namespace: Microsoft. Graph

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
