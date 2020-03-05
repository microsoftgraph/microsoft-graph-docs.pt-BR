---
title: tipo de recurso protectByTemplateAction
description: Informa ao aplicativo que um modelo de proteção de proteção de informações do Azure deve ser aplicado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3fc936179a0c0764492a3dc8d677060931a1223a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521366"
---
# <a name="protectbytemplateaction-resource-type"></a>tipo de recurso protectByTemplateAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informa ao aplicativo que um modelo de proteção de proteção de informações do Azure deve ser aplicado. **protectionByTemplateAction** pode ser retornado por [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) ou [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) se o rótulo resultante tiver sido configurado para aplicar proteção. O aplicativo de consumo deve ler o TemplateID do resultado e, em seguida, usar uma biblioteca de cliente, como o SDK do Microsoft Information Protection, para aplicar proteção por meio da proteção de informações do Azure.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo   | Descrição                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| templateId | String | O GUID do modelo de proteção de informações do Azure a ser aplicado às informações. |

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