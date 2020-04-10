---
title: tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12f1a38340b4c341d65930000c22a6cd2daeb567
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219169"
---
# <a name="attributemappingparameterschema-resource-type"></a>tipo de recurso attributeMappingParameterSchema

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Boolean                   |O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres `Concatenate(string,string,...)` de entrada na função). |
|nome                        |String                    |Nome do parâmetro. |
|obrigatório                    |Boolean                   |`true`Se o parâmetro for necessário; caso `false`contrário. |
|tipo                        |String                    |Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`. O padrão é `String`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
