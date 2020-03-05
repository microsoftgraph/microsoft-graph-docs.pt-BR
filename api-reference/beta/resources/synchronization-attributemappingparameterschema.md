---
title: tipo de recurso attributeMappingParameterSchema
description: Descreve um único parâmetro usado em um attributeMappingFunctionSchema.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d4415c6ece2fc9095070eb888ad4bd7bba583d54
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520237"
---
# <a name="attributemappingparameterschema-resource-type"></a>tipo de recurso attributeMappingParameterSchema

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um único parâmetro usado em um [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Boolean                   |O parâmetro fornecido pode ser fornecido várias vezes (por exemplo, várias cadeias de caracteres `Concatenate(string,string,...)` de entrada na função). |
|nome                        |String                    |Nome do parâmetro. |
|obrigatório                    |Boolean                   |`true`Se o parâmetro for necessário; caso `false`contrário. |
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
  "suppressions": []
}
-->
