---
title: Tipo de recurso addWatermarkAction
description: Representa uma ação que especifica os detalhes sobre a marca d'água do conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db493c57d6de7c840e5f0606743392698cb475b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962123"
---
# <a name="addwatermarkaction-resource-type"></a>Tipo de recurso addWatermarkAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes sobre a marca d'água do conteúdo a ser adicionado às informações, se aplicável.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo   | Descrição                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| fontColor     | Cadeia de caracteres | Cor da fonte a ser usada para a marca d'água.                      |
| fontName      | Cadeia de caracteres | Nome da fonte a ser usada para a marca d'água.                       |
| fontSize      | Int32  | Tamanho da fonte a ser usado para a marca d'água.                              |
| layout        | String | Os valores possíveis são: `horizontal` e `diagonal`.                   |
| texto          | Cadeia de caracteres | O conteúdo da marca d'água em si.                            |
| uiElementName | Cadeia de caracteres | O nome do elemento da interface do usuário onde a marca d'água deve ser colocada. |

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

