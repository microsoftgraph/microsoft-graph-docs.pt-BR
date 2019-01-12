---
title: tipo de recurso de imageInfo
description: Um tipo complexo para representar a propriedade **atribuição** na parte visualInfo do objeto atividade.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 347e07b70e8bad6dce8571dd1fbac5cd00d9abdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978687"
---
# <a name="imageinfo-resource-type"></a>tipo de recurso de imageInfo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um tipo complexo para representar a propriedade **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [atividade](../resources/projectrome-activity.md) .

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|iconUrl | Cadeia de caracteres | Opcional; URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade|
|alternateText | Cadeia de caracteres | Opcional; conteúdo de texto ALT acessível para a imagem|
|addImageQuery | Booliano | Opcional; parâmetro usado para indicar o servidor é capaz de processar imagem dinamicamente em resposta às parametrização. Por exemplo, – uma imagem de alto contraste|

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
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
