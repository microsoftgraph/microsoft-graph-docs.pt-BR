---
title: tipo de recurso synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a754b03379d1e40ba7310283a0efdd94ff30631
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520076"
---
# <a name="synchronizationerror-resource-type"></a>tipo de recurso synchronizationError

Namespace: Microsoft. Graph

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
