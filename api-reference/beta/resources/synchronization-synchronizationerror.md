---
title: Tipo de recurso synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a49f2cf9b9d3e621533490127a5b2674ab43bf14
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131485"
---
# <a name="synchronizationerror-resource-type"></a>Tipo de recurso synchronizationError

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro que ocorreu durante o processo de sincronização.

## <a name="properties"></a>Propriedades

<!-- Add descriptions for the properties. -->
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|código|String||
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


