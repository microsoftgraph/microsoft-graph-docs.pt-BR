---
title: Tipo de recurso expressionInputObject
description: Representa um objeto a ser usado como dados de teste de entrada quando a ação synchronizationSchema parseExpression executa uma avaliação de expressão.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 161589d9d8b6e3d06ef6afe31df0fde79bf938bb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132045"
---
# <a name="expressioninputobject-resource-type"></a>Tipo de recurso expressionInputObject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto a ser usado como dados de teste de entrada quando a [ação parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) executa uma avaliação de expressão.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definição|[objectDefinition](synchronization-objectdefinition.md)|Definição do objeto de teste.|
|properties|[Coleção stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)|Valores de propriedade do objeto de teste.|

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


