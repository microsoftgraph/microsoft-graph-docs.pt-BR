---
title: tipo de recurso metadataaction
description: Representa os metadados a serem gravados ou removidos de um arquivo.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8652a33de04d0a28a34c3738dd1706d6aff5e5b9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938902"
---
# <a name="metadataaction-resource-type"></a>tipo de recurso metadataaction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os metadados a serem gravados ou removidos de um arquivo. **metadataaction** pode ser retornado pelas APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) . A ação informa o aplicativo de consumo dos pares chave/valor específicos que devem ser adicionados ao arquivo ou as chaves de metadados específicas que devem ser removidas do arquivo. Este metadados é o que descreve o arquivo ou as informações que estão sendo *rotuladas*.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                                       | Descrição                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| metadataToAdd    | Coleção [keyValuePair](keyvaluepair.md) | Uma coleção de pares chave de valor que deve ser adicionado ao arquivo.                  |
| metadataToRemove | String collection                          | Uma coleção de cadeias de caracteres que indicam quais teclas serão removidas dos metadados do arquivo. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "metadataToAdd": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "metadataToRemove": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->