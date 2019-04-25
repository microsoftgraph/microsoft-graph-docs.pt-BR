---
title: tipo de recurso attributeMapping
description: Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582083"
---
# <a name="attributemapping-resource-type"></a>tipo de recurso attributeMapping

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
