---
title: tipo de recurso de visualInfo
description: Um tipo complexo para representar a propriedade **visualElements** no objeto de atividade.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 416109bb1bb6625330ddfbbb32b8fb688b223134
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962643"
---
# <a name="visualinfo-resource-type"></a>tipo de recurso de visualInfo

Um tipo complexo para representar a propriedade **visualElements** no objeto de [atividade](../resources/projectrome-activity.md) .

Cada atividade do usuário será exibida na linha do tempo como um cartão adaptável. Desenvolvedores de aplicativos são incentivados a fornecer um cartão personalizado que captura a essência da atividade que foi realizada no seu aplicativo. Isso é possível, fornecendo um cartão JSON personalizado na propriedade conteúdo.

Além dos metadados visual com uma placa adaptável, app pode especificar metadados do conteúdo – dados a ser usado para construir Inferências sobre a atividade do usuário a fim de oferecer novas atividades para o compromisso re futura. Isso é possível usando a propriedade de contentInfo da atividade para fornecer um objeto JSON que aproveita as propriedades de schema.org para descrever o conteúdo.

Se não for fornecido um cartão personalizado, será gerado um cartão simple usando propriedades displayText e descrição. Cartões personalizados são recomendados para demonstrar o melhor conteúdo de dentro de seu aplicativo.

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:------|:-----------|
|displayText | String | Obrigatório. Uma breve descrição de texto de atividade de exclusivo do usuário (por exemplo, nome do documento em casos onde uma atividade refere-se a criação de documentos)|
|description | String | Opcional. Descrição de texto mais longa da atividade exclusivo do usuário (exemplo: nome, primeira frase e/ou metadados de documentos)|
|backgroundColor | String | Opcional. Cor de plano de fundo usada para processar a atividade na interface do usuário - cor de marca para a fonte da atividade do aplicativo. Deve ser uma cor hexadecimal válida|
|content | Objeto sem JSON | Opcional. Parte personalizada de dados - objeto JSON usados para fornecer conteúdo personalizado para renderizar a atividade no UI do Shell do Windows|
|attribution | [imageInfo](../resources/projectrome-imageinfo.md) | Opcional. Objeto JSON usado para representar um ícone que representa o aplicativo usado para gerar a atividade|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
