---
title: Tipo de recurso protectDoNotForwardAction
description: Informa ao aplicativo para aplicar a proteção Não Encaminhar.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a68771ea278ba8a904c032a86732b2b190eeeb43
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941768"
---
# <a name="protectdonotforwardaction-resource-type"></a>Tipo de recurso protectDoNotForwardAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informa ao aplicativo para aplicar a proteção Não Encaminhar. **protectionDoNotForwardAction** poderá ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar a proteção [Não Encaminhar](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails). O aplicativo de consumo deve usar uma biblioteca de clientes para aplicar proteção por meio da Proteção de Informações do Azure.

## <a name="properties"></a>Propriedades

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectDoNotForwardAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectDoNotForwardAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->