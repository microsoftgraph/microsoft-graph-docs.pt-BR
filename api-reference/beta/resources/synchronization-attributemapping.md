---
title: Tipo de recurso attributeMapping
description: Define como os valores para o atributo de destino determinado devem fluir durante a sincronização.
ms.localizationpriority: medium
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d66937d1951bd3fa65db6f17b70fd0df2a6de534
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224766"
---
# <a name="attributemapping-resource-type"></a>Tipo de recurso attributeMapping

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define como os valores para o atributo de destino determinado devem fluir durante a sincronização.

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                      | Descrição    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | Cadeia de Caracteres                    |Valor padrão a ser usado caso a **propriedade de origem** tenha sido avaliada como `null` . Opcional.|
|exportMissingReferences    |Booleano                     |Apenas para uso interno.|
|flowBehavior               |attributeFlowBehavior      |Define quando esse atributo deve ser exportado para o diretório de destino. Os valores possíveis são: `FlowWhenChanged` e `FlowAlways` . O padrão é `FlowWhenChanged`. |
|flowType                   |attributeFlowType          |Define quando esse atributo deve ser atualizado no diretório de destino. Os valores possíveis são: (padrão), (somente quando novo objeto é criado), (somente quando a alteração está adicionando novos valores a um atributo `Always` `ObjectAddOnly` de vários `MultiValueAddOnly` valores). |
|matchingPriority           |Int32                      |Se for maior que 0, esse atributo será usado para executar uma combinação inicial dos objetos entre diretórios de origem e destino. O mecanismo de sincronização tentará encontrar o objeto correspondente usando o atributo com o menor valor de prioridade correspondente primeiro. Se não for encontrado, o atributo com a próxima prioridade correspondente será usado e, assim, até que a correspondência seja encontrada ou não mais atributos correspondentes sejam deixados. Somente atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | Define como um valor deve ser extraído (ou transformado) do objeto de origem. |
|targetAttributeName        |Cadeia de Caracteres                     |Nome do atributo no objeto de destino. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": "Boolean",
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


