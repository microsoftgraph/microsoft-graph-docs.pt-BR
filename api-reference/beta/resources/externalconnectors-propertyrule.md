---
title: Tipo de recurso propertyRule
description: Define o conjunto de condições para exibir um displayTemplate
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7f1e021e4bc735ff7f5efd322e0a5a8080e5816b
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214911"
---
# <a name="propertyrule-resource-type"></a>Tipo de recurso propertyRule

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o conjunto de condições para exibir [um displayTemplate](../resources/externalconnectors-displaytemplate.md). As regras usam o formato: (propriedade do esquema do item) + (operação) + (valor). Por exemplo, uma **propriedadeRule** pode especificar que "itemTitle" "contém" "contoso". Portanto, **o displayTemplate** não será exibido, a menos que itemTitle contenha o valor "contoso".

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|operation|String|Especifica as operações a serem executadas durante a avaliação de uma única **propriedadeRule**, onde e uma cadeia de caracteres da `property` coleção são os `values` respectivos operands. Os valores possíveis são: `null`, `equals`, `notEquals`, `contains`, `notContains`, `lessThan`, `greaterThan`, `startsWith`, `unknownFutureValue`. Obrigatório.|
|propriedade|Cadeia de caracteres|A propriedade do [esquema externalItem.](../resources/externalconnectors-externalitem.md) Obrigatório.|
|values|Coleção de cadeias de caracteres|Uma coleção com uma ou muitas cadeias de caracteres. As cadeias de caracteres especificadas serão corresponder à propriedade especificada usando a operação especificada. Obrigatório.|
|valuesJoinedBy|binaryOperator|O operador de junção para avaliar várias **propriedadesRules**. Por exemplo, se for especificado, todas as `and` **propriedadesRules** devem ser verdadeiras para que **a propriedadeRule** seja true. Os valores possíveis são: `or` e `and`. Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.propertyRule"
}
-->
``` json
{
  "property": "String",
  "operation": "String",
  "valuesJoinedBy": "String",
  "values": [
    "String"
  ]
}
```

