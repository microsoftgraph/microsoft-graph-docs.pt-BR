---
title: Tipo de recurso metadataAction
description: Representa os metadados a serem gravados ou removidos de um arquivo.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 23305d8a3e1e89d198b4700e794dd264eabf003b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960394"
---
# <a name="metadataaction-resource-type"></a>Tipo de recurso metadataAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os metadados a serem gravados ou removidos de um arquivo. **metadataAction** pode ser retornada pelas APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [evaluateClassificationResults.](../api/informationprotectionlabel-evaluateclassificationresults.md) A ação informa o aplicativo de consumo dos pares de chave/valor específicos que devem ser adicionados ao arquivo ou às chaves de metadados específicas que devem ser removidas do arquivo. Esse metadados é o que descreve o arquivo ou informações como *sendo rotulados*.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                                       | Descrição                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| metadataToAdd    | Coleção [keyValuePair](keyvaluepair.md) | Uma coleção de pares de valores-chave que devem ser adicionados ao arquivo.                  |
| metadataToRemove | Coleção de cadeias de caracteres                          | Uma coleção de cadeias de caracteres que indica quais chaves remover dos metadados do arquivo. |

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

