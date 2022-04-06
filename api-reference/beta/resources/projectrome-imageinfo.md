---
title: Tipo de recurso imageInfo
description: Um tipo complexo para representar **a propriedade de atribuição** na parte visualInfo do objeto activity.
ms.localizationpriority: medium
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: a123ea442fe4309ea96962b4155e0f36909fee7b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723767"
---
# <a name="imageinfo-resource-type"></a>Tipo de recurso imageInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo complexo para representar **a propriedade de atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do [objeto activity](../resources/projectrome-activity.md) .

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo    | Descrição                                                                                                                                              |
| :------------ | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------- |
| iconUrl       | String  | Opcional; URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade                                                      |
| alternateText | String  | Opcional; alt-text accessible content for the image                                                                                                      |
| addImageQuery | Booliano | Opcional; usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização. Por exemplo: uma imagem de alto contraste |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
