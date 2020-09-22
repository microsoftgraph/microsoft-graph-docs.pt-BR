---
title: tipo de recurso addContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4e9edf4007d7bc5d4028e4f9202e09647ca863
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024511"
---
# <a name="addcontentfooteraction-resource-type"></a>tipo de recurso addContentFooterAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser adicionado às informações, se aplicável.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo   | Descrição                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| Alinhamento     | String | Os valores possíveis são: `left`, `right`, `center`.               |
| fontColor     | String | Cor da fonte a ser usada para o rodapé.                      |
| fontName      | String | Nome da fonte a ser usada para o rodapé.                       |
| fontSize      | Int32  | Tamanho da fonte a ser usado para o rodapé.                              |
| margin        | Int32  | A margem do cabeçalho na parte inferior do documento.     |
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

