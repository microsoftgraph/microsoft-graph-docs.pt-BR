---
title: tipo de recurso de attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529947"
---
# <a name="attributemappingparameterschema-resource-type"></a>tipo de recurso de attributeMappingParameterSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Booliano                   |O parâmetro determinado pode ser fornecido várias vezes (por exemplo, a entrada de vários strings no `Concatenate(string,string,...)` função). |
|name                        |Cadeia de caracteres                    |Nome do parâmetro |
|obrigatório                    |Booliano                   |`true`Se o parâmetro é obrigatório; Caso contrário, `false`. |
|type                        |String                    |Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`. O padrão é `String`.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingparameterschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
