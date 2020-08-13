---
title: tipo de recurso addwatermarkaction
description: Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a94f517fe9f5da207febf9e776643a7c17c18d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508398"
---
# <a name="addwatermarkaction-resource-type"></a>tipo de recurso addwatermarkaction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser adicionado às informações, se aplicável.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo   | Descrição                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| fontColor     | String | Cor da fonte a ser usada para a marca d' água.                      |
| fontName      | String | Nome da fonte a ser usada para a marca d' água.                       |
| fontSize      | Int32  | Tamanho da fonte a ser usado para a marca d' água.                              |
| teclado        | String | Os valores possíveis são: `horizontal` e `diagonal`.                   |
| texto          | String | O conteúdo da própria marca d' água.                            |
| uiElementname | String | O nome do elemento de interface do usuário onde a marca d' água deve ser colocada. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "layout": "String",
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addWatermarkAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->