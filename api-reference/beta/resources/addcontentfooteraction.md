---
title: tipo de recurso addContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b1a2cb0f3e2ffbfb5554c4ae0323cf4fd028e0c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939100"
---
# <a name="addcontentfooteraction-resource-type"></a>tipo de recurso addContentFooterAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser adicionado às informações, se aplicável.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo   | Descrição                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| Alinhamento     | String | Os valores possíveis são: `left`, `right`, `center`.               |
| fontColor     | String | Cor da fonte a ser usada para o rodapé.                      |
| fontName      | String | Nome da fonte a ser usada para o rodapé.                       |
| fontSize      | Int32  | Tamanho da fonte a ser usado para o rodapé.                              |
| Margin        | Int32  | A margem do cabeçalho na parte inferior do documento.     |
| texto          | String | O conteúdo do rodapé propriamente dito.                            |
| uiElementname | String | O nome do elemento de interface do usuário onde o rodapé deve ser colocado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentFooterAction",
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
  "description": "addContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->