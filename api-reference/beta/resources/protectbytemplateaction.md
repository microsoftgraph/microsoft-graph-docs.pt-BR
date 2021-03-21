---
title: Tipo de recurso protectByTemplateAction
description: Informa ao aplicativo que um modelo de proteção de informações do Azure deve ser aplicado.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6524774af3faa496b141e37ec270f8a73770ee63
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956824"
---
# <a name="protectbytemplateaction-resource-type"></a>Tipo de recurso protectByTemplateAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informa ao aplicativo que um modelo de proteção de informações do Azure deve ser aplicado. **protectionByTemplateAction** pode ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar proteção. O aplicativo de consumo deve ler o templateId do resultado e, em seguida, usar uma biblioteca de clientes, como o SDK da Proteção de Informações da Microsoft, para aplicar proteção por meio da Proteção de Informações do Azure.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo   | Descrição                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| templateId | Cadeia de caracteres | O GUID do modelo de Proteção de Informações do Azure a ser aplicado às informações. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectByTemplateAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "templateId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectByTemplateAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

