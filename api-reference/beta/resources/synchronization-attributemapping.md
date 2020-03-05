---
title: tipo de recurso attributeMapping
description: Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e200fdf9c7a3d48945ff0d5e2cb080c7b6774e9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520251"
---
# <a name="attributemapping-resource-type"></a>tipo de recurso attributeMapping

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                      | Descrição    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | String                    |Valor padrão a ser usado no caso de a propriedade **Source** ter sido `null`avaliada. Opcional.|
|exportMissingReferences    |String                     |Apenas para uso interno.|
|flowBehavior               |attributeFlowBehavior      |Define quando esse atributo deve ser exportado para o diretório de destino. Os valores possíveis são `FlowWhenChanged` : `FlowAlways`e. O padrão é `FlowWhenChanged`. |
|flowtype                   |attributeFlowType          |Define quando esse atributo deve ser atualizado no diretório de destino. Os valores possíveis são `Always` : (padrão) `ObjectAddOnly` , (somente quando novo objeto é criado) `MultiValueAddOnly` , (somente quando a alteração está adicionando novos valores a um atributo com valores múltiplos). |
|matchingPriority           |Int32                      |Se for maior que 0, este atributo será usado para executar uma correspondência inicial dos objetos entre os diretórios de origem e de destino. O mecanismo de sincronização tentará localizar o objeto correspondente usando o atributo com o menor valor de prioridade correspondente primeiro. Se não for encontrado, será usado o atributo com a próxima prioridade correspondente e, assim, em um até que a correspondência seja encontrada ou nenhum outro atributo de correspondência seja deixado. Somente atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | Define como um valor deve ser extraído (ou transformado) a partir do objeto Source. |
|targetAttributeName        |String                     |Nome do atributo no objeto de destino. |

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
  "exportMissingReferences": true,
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
