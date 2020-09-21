---
title: tipo de recurso expressionInputObject
description: Representa um objeto a ser usado como dados de teste de entrada quando a ação synchronizationSchema ParseName executa uma avaliação de expressão.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9727f50b05eb8cdb5319883dd0058a91d9383cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968350"
---
# <a name="expressioninputobject-resource-type"></a>tipo de recurso expressionInputObject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto que será usado como dados de teste de entrada quando a ação [parsetable](../api/synchronization-synchronizationschema-parseexpression.md) executar uma avaliação de expressão.

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


