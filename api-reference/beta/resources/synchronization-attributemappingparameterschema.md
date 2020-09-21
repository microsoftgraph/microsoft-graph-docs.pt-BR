---
title: tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32710c5411f054ad096bdd293a2f7d46e89a6944
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078071"
---
# <a name="attributemappingparameterschema-resource-type"></a>tipo de recurso attributeMappingParameterSchema

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Booliano                   |O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres de entrada na `Concatenate(string,string,...)` função). |
|name                        |Cadeia de caracteres                    |Nome do parâmetro. |
|obrigatório                    |Booliano                   |`true` Se o parâmetro for necessário; caso contrário `false` . |
|tipo                        |Cadeia de caracteres                    |Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`. O padrão é `String`.|

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


