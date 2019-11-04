---
title: tipo de recurso contentInfo
description: Representa o estado atual de algumas informações que serão rotuladas.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5191be0533810f0a9da3b0ea83f209d69cc67297
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938874"
---
# <a name="contentinfo-resource-type"></a>tipo de recurso contentInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado atual de algumas informações que serão rotuladas. **contentInfo** é passado para as APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) para descrever a API o estado atual das informações. Este detalhe de **contentInfo** orienta os resultados em quais metadados, a marcação de conteúdo e a proteção devem ser adicionados ou removidos quando o rótulo é aplicado, atualizado ou removido. 

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                                       | Descrição                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| formato     | String                                     | Os valores possíveis são: `default` e `email`.                                                                                        |
| identificador | String                                     | Identificador usado para a análise de proteção de informações do Azure.                                                                     |
| los   | Coleção [keyValuePair](keyvaluepair.md) | Os metadados de proteção de informações existentes da Microsoft são passados como pares chave/valor, onde a chave é o MSIP_Label_GUID_PropName. |
| state      | String                                     | Os valores possíveis são: `rest`, `motion`, `use`.                                                                                   |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.contentInfo",
  "baseType": null
}-->

```json
{
  "format": "String",
  "identifier": "String",
  "metadata": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contentInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->