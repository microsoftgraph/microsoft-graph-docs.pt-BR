---
title: tipo de recurso de expressionInputObject
description: 'Representa um objeto a ser usado como dados de teste de entrada quando a [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação realiza uma avaliação de expressão.'
localization_priority: Normal
ms.openlocfilehash: acf0fa5125d863224de6df76d46109b9888f8ddf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820108"
---
# <a name="expressioninputobject-resource-type"></a>tipo de recurso de expressionInputObject

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um objeto a ser usado como dados de teste de entrada quando a [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação realiza uma avaliação de expressão.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definição|[objectDefinition](synchronization-objectdefinition.md)|Definição do objeto de teste.|
|properties|coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)|Valores de propriedade do objeto de teste.|

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
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
