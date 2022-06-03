---
title: Tipo de recurso contentInfo
description: Representa o estado atual de algumas informações que devem ser rotuladas.
ms.localizationpriority: medium
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7dc6c99e1c4c19564e17c406beca02971071c671
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884171"
---
# <a name="contentinfo-resource-type"></a>Tipo de recurso contentInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado atual de algumas informações que devem ser rotuladas. **contentInfo** é passado para as APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md) e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) para descrever para a API o estado atual das informações. Este **detalhe contentInfo** orienta os resultados sobre quais metadados, marcação de conteúdo e proteção devem ser adicionados ou removidos quando o rótulo é aplicado, atualizado ou removido. 

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                                       | Descrição                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| formato     | String                                     | Os valores possíveis são: `default` e `email`.                                                                                        |
| identificador | String                                     | Identificador usado para a Análise de Proteção de Informações do Azure.                                                                     |
| Metadados   | Coleção [keyValuePair](keyvaluepair.md) | Os metadados existentes da Proteção de Informações do Microsoft Purview são passados como pares chave-valor, em que a chave é a MSIP_Label_GUID_PropName. |
| estado      | String                                     | Os valores possíveis são: `rest`, `motion`, `use`.                                                                                   |

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

