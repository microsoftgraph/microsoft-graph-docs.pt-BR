---
title: tipo de recurso expressionInputObject
description: 'Representa um objeto a ser usado como dados de teste de entrada quando a ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) executa uma avaliação de expressão.'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 113c38e540b8c41fb3d3156b27f6f5e1f1df42f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007946"
---
# <a name="expressioninputobject-resource-type"></a>tipo de recurso expressionInputObject

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto que será usado como dados de teste de entrada [](../api/synchronization-synchronizationschema-parseexpression.md) quando a ação parsetable executar uma avaliação de expressão.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definir|[ObjectDefinition](synchronization-objectdefinition.md)|Definição do objeto Test.|
|properties|coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)|Valores de Propriedade do objeto Test.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
