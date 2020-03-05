---
title: tipo de recurso addContentHeaderAction
description: Representa uma ação que especifica os detalhes sobre o cabeçalho de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d426252b6ab83557c3d3085ac4ffa7a530aae271
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508405"
---
# <a name="addcontentheaderaction-resource-type"></a>tipo de recurso addContentHeaderAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes sobre o cabeçalho de conteúdo a ser adicionado às informações, se aplicável.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo   | Descrição                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| Alinhamento     | String | Os valores possíveis são: `left`, `right`, `center`.               |
| fontColor     | String | Cor da fonte a ser usada para o cabeçalho.                      |
| fontName      | String | Nome da fonte a ser usada para o cabeçalho.                       |
| fontSize      | Int32  | Tamanho da fonte a ser usado para o cabeçalho.                              |
| Margin        | Int32  | A margem do cabeçalho na parte superior do documento.        |
| texto          | String | O conteúdo do próprio cabeçalho.                            |
| uiElementname | String | O nome do elemento de interface do usuário onde o cabeçalho deve ser colocado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentHeaderAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "alignment": "String",
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "margin": 1024,
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->