---
title: tipo de recurso de attributeMapping
description: Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: 6c7a6367684b3e11013355b6d4726afe3346dab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825274"
---
# <a name="attributemapping-resource-type"></a>tipo de recurso de attributeMapping

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                      | Descrição    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | String                    |Valor a ser usado caso a propriedade **source** foi avaliada como padrão `null`. Opcional.|
|exportMissingReferences    |Cadeia de caracteres                     |Apenas para uso interno.|
|flowBehavior               |attributeFlowBehavior      |Define quando este atributo deve ser exportado para o diretório de destino. Os valores possíveis são: `FlowWhenChanged` e `FlowAlways`. O padrão é `FlowWhenChanged`. |
|flowType                   |attributeFlowType          |Define quando este atributo deve ser atualizado no diretório de destino. Os valores possíveis são: `Always` (padrão), `ObjectAddOnly` (somente quando novo objeto é criado), `MultiValueAddOnly` (somente quando a alteração é adicionando novos valores para um atributo de valores múltiplos). |
|matchingPriority           |Int32                      |Se for maior do que 0, esse atributo será usado para executar uma correspondência inicial dos objetos entre os diretórios de origem e destino. O mecanismo de sincronização tentará localizar o objeto correspondente usando o atributo com menor valor de prioridade de correspondência pela primeira vez. Se não encontrado, o atributo com a prioridade de correspondência próxima será usado e assim por diante um até correspondência for encontrada ou não mais atributos correspondentes são deixados. Apenas os atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | Define como um valor deve ser extraída (ou transformados) do objeto de origem. |
|targetAttributeName        |Cadeia de caracteres                     |Nome do atributo no objeto de destino. |

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
