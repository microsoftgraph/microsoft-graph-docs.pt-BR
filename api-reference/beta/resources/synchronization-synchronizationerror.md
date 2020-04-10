---
title: tipo de recurso synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 884c39273d8d474a228cd8f4a8f2b321950e8caf
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217546"
---
# <a name="synchronizationerror-resource-type"></a>tipo de recurso synchronizationError

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro que ocorreu durante o processo de sincronização.

## <a name="properties"></a>Propriedades

<!-- Add descriptions for the properties. -->
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|código|Cadeia de Caracteres||
|mensagem|String||
|tenantActionable|Boolean||

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
