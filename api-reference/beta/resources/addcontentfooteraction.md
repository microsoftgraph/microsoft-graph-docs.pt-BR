---
title: Tipo de recurso addContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a serem adicionados às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 20debce7dc408bd10d4f62b905efa55156d4d4ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962131"
---
# <a name="addcontentfooteraction-resource-type"></a>Tipo de recurso addContentFooterAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que especifica os detalhes no rodapé de conteúdo a serem adicionados às informações, se aplicável.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo   | Descrição                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| Alinhamento     | Cadeia de caracteres | Os valores possíveis são: `left`, `right`, `center`.               |
| fontColor     | Cadeia de caracteres | Cor da fonte a ser usada para o rodapé.                      |
| fontName      | Cadeia de caracteres | Nome da fonte a ser usada para o rodapé.                       |
| fontSize      | Int32  | Tamanho da fonte a ser usado para o rodapé.                              |
| margin        | Int32  | A margem do header na parte inferior do documento.     |
| texto          | Cadeia de caracteres | O conteúdo do rodapé em si.                            |
| uiElementName | Cadeia de caracteres | O nome do elemento da interface do usuário onde o rodapé deve ser colocado. |

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

