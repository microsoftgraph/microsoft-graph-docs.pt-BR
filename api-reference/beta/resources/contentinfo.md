---
title: Tipo de recurso contentInfo
description: Representa o estado atual de algumas informações que devem ser rotuladas.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 939d7730c0de2ffb13d4dbdcade6f7c2fbce5de4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962648"
---
# <a name="contentinfo-resource-type"></a>Tipo de recurso contentInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado atual de algumas informações que devem ser rotuladas. **contentInfo** é passado para as APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) para descrever para a API o estado atual das informações. Este **detalhe contentInfo** orienta os resultados sobre quais metadados, marcação de conteúdo e proteção devem ser adicionados ou removidos quando o rótulo for aplicado, atualizado ou removido. 

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                                       | Descrição                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| formato     | String                                     | Os valores possíveis são: `default` e `email`.                                                                                        |
| identificador | Cadeia de caracteres                                     | Identificador usado para o Azure Information Protection Analytics.                                                                     |
| metadados   | Coleção [keyValuePair](keyvaluepair.md) | Os metadados existentes da Proteção de Informações da Microsoft são passados como pares de chave/valor, onde a chave é a MSIP_Label_GUID_PropName. |
| estado      | Cadeia de caracteres                                     | Os valores possíveis são: `rest`, `motion`, `use`.                                                                                   |

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

